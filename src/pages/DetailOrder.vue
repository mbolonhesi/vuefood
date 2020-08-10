<template>
    <div>
        <div class="row my-4 mx-0 details">
      <div class="col-12 mb-2">
        <h1 class="title-tenant h2">Detalhes do Pedido <strong>dasfdsafda</strong></h1>
      </div>
      <div class="col-sm-6">
        <ul class="p-0">
          <li><b>Número:</b> dfdsafsa</li>
          <li><b>Total:</b> R$ 78,00</li>
          <li><b>Data:</b> 20/20/2020</li>
          <li><b>Status:</b> <span class="badge bg-success text-light p-2">Em Aberto</span></li>
        </ul>
      </div>
      <div class="col-sm-6">
        <ul class="p-0">
          <li>
            <span>Mesa</span>
            <ul class="p-0">
              <li><b>Identificador:</b> sdfds</li>
              <li><b>Descrição:</b> sdfds</li>
            </ul>
          </li>
          <li>
            <span>Cliente</span>
            <ul class="p-0">
              <li><b>Nome:</b> Carlos</li>
              <li><b>E-mail:</b> carlos@especializati.com.br</li>
            </ul>
          </li>
        </ul>
      </div>
    </div> <!-- details order -->

    <hr>

    <div class="row my-4">
      <div class="col-12">
        <h4>Produtos</h4>
      </div>

        <div class="col-12 col-md-6 col-lg-4 my-1">
          <div class="details-card">
            <a href="vitrine-tenant.html"><img class="card-img-top" src="imgs/pizza.png" alt=""></a>
            <div class="details-card-body">
              <h5>Pizza</h5>
              <p><b>R$: 10,00</b></p>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6 col-lg-4 my-1">
          <div class="details-card">
            <a href="vitrine-tenant.html"><img class="card-img-top" src="imgs/pizza.png" alt=""></a>
            <div class="details-card-body">
              <h5>Pizza</h5>
              <p><b>R$: 10,00</b></p>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-6 col-lg-4 my-1">
          <div class="details-card">
            <a href="vitrine-tenant.html"><img class="card-img-top" src="imgs/pizza.png" alt=""></a>
            <div class="details-card-body">
              <h5>Pizza</h5>
              <p><b>R$: 10,00</b></p>
            </div>
          </div>
        </div>

    </div>
    <!-- products order -->
    </div>
</template>

<script>
export default {
    props: ['identify'],
    created() {
        console.log(this.identify);
    }
}
</script>