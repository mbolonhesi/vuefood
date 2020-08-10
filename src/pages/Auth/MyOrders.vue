<template>
    <div>
         <div class="my-4">
      <h1 class="title-tenant">Meus Pedidos</h1>
    </div>

    <div class="my-orders my-4">
      <div class="my-table-header mb-4">
        <div class="text-center"><b>Nª Pedido</b></div>
        <div class="text-center"><b>Data</b></div>
        <div class="text-center"><b>Valor Total</b></div>
        <div class="text-center"><b>Detalhes</b></div>
      </div>

      <div class="my-table " v-for="(order, index) in myOrders.data" :key="index">
        <div class="text-center"><b>{{ order.identify }}</b></div>
        <div class="text-center">{{ order.date }}</div>
        <div class="text-center">R$: {{ order.price }} </div>
        <div class="text-center"><a href="detalhes-pedido.html" class="btn btn-danger">Detalhes</a></div>
      </div>
      
    </div>
    </div>
</template>

<script>
import { mapActions, mapState} from 'vuex'

export default {
    create(){
        this.getMyOrders()
              .catch(_ => this.$vToastify.error("Falha ao buscar os pedidos",'Erro'))
    },
    computed:{
        ...mapState({
            myOrders: state => state.orders.myOrders
        }),
    },
    methods:{
        ...mapActions([
            'getMyOrders'
        ]),
    },
}
</script>