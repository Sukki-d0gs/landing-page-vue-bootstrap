<template>
    <div class="container">
        <div class="row text-center">
            <div class="col d-flex justify-content-center">
                <div class="card" style="width: 13rem;">
                    <img src="data:image/jpeg;base64,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" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">Morrocan coffee</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="btn btn-primary">1.99$</a>
                    </div>
                </div>
            </div>
            <div class="col d-flex justify-content-center">
                <div class="card" style="width: 13rem;">
                    <img style="height: 13rem;" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/Rafcoffe.jpg/220px-Rafcoffe.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">Hot Chockolate</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="btn btn-primary">0.99$</a>
                    </div>
                </div>
            </div>
            <div class="col d-flex justify-content-center">
                <div class="card" style="width: 13rem;">
                    <img src="https://images.wsj.net/im-404844?width=1280&size=1" class="card-img-top" style="height: 13rem;">
                    <div class="card-body">
                        <h5 class="card-title">Turkish coffee</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="btn btn-primary">2.99$</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .card {
        cursor: pointer;
    }
</style>