<template>
    <div class="container-fluid">
        <div class="row mb-2 mt-3">
            <div class="col-12">
                <div class="card shadow">
                    <div class="row no-gutters">
                        <div class="d-none d-lg-block col-lg-1 col-xl-2"></div>
                        <div class="col-12 col-sm-12 col-md-4 col-lg-4 col-xl-4 mt-5">
                            <h3 class="mt-2 ml-3">
                                <span class="text-success"><i class="far fa-clock"></i></span>
                                Programare
                            </h3>
                            <p class="ml-3">Programeaza-te online si beneficiaza de un discount de 10%</p>
                            <div class="form-group mt-5 ml-3">
                                <label for="name">
                                    <h5>
                                        <span class="text-success">
                                            <i class="fas fa-signature"></i>
                                        </span>
                                        Nume
                                    </h5>
                                </label>
                                <input type="text" class="form-control">
                            </div>
                            <div class="form-group mt-5 ml-3">
                                <label for="ora">
                                    <h5>
                                        <span class="text-success">
                                            <i class="far fa-calendar-plus"></i>
                                        </span>
                                        Alege ora si data
                                    </h5>
                                </label>
                                <input type="text" class="form-control" id="ora" v-on:focus="test()">
                            </div>
                            <button class="btn btn-block btn-success mt-5">
                                <i class="fas fa-share-square"></i>
                                Programeaza
                            </button>
                        </div>
                        <div class="d-none d-lg-block col-lg-1 col-xl-1"></div>
                        <div class="d-none d-md-block col-md-8 col-lg-6 col-xl-5">
                            <img src="../assets/manichure-left.png" class="card-img" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
// import flatpickr from 'flatpickr';
// import '../../node_modules/flatpickr/dist/flatpickr.min.css';
import TinyDatePicker from 'tiny-date-picker';
import '../../node_modules/tiny-date-picker/tiny-date-picker.css';

export default {
    name: "Programare",
    methods: {
        test(){
            console.log('test');
            //flatpickr('#ora');
            TinyDatePicker('#ora');
        }
    }
}
</script>

<style scoped>
    
</style>