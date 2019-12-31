<template>
    <div>
        <base-header class="header pb-8 pt-5 pt-lg-8 d-flex align-items-center"
                     style="min-height: 600px; background-image: url(); background-size: cover; background-position: center top;"> 
            <!-- Mask -->
            <span class="mask bg-gradient-success opacity-8"></span>
            <!-- Header container -->
            <div class="container-fluid d-flex align-items-center">
                <div class="row">
                    <div class="col-lg-7 col-md-10">
                        <h1 class="display-2 text-white">Ajoutez des étudiants plus rapidement!</h1>
                        <p class="text-white mt-0 mb-5">Cette partie de l'application permet à un administrateur d'ajouter un étudiant.</p>
                        
                    </div>
                </div>
            </div>
        </base-header>

        <div class="container-fluid mt--7">
            <div class="row">
                <div class="col-xl-4 order-xl-2 mb-5 mb-xl-0">

                   
                </div>

                <div class="col-xl-8 order-xl-1">
                    <card shadow type="secondary">
                        <div slot="header" class="bg-white border-0">
                            <div class="row align-items-center">
                                <div class="col-8">
                                    <h3 class="mb-0">Ajouter un étudiant</h3>
                                </div>
                                <div class="col-4 text-right">
                                    <a href="#!" class="btn btn-sm btn-primary">Paramètres</a>
                                </div>
                            </div>
                        </div>
                        <template>
                            <form @submit.prevent>
                                <h6 class="heading-small text-muted mb-4">Informations étudiant</h6>
                                <div class="pl-lg-4">
                                    <div class="row">
                                        <div class="col-lg-6">
                                            <base-input alternative=""
                                                        label="Matricule"
                                                        placeholder="année bac/ rang"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.matricule"
                                            />
                                        </div>
                                        <div class="col-lg-6">
                                            <base-input alternative=""
                                                        label="Adresse mail"
                                                        placeholder="ex: hi_kara@esi.dz"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.email"
                                            />
                                        </div>
                                    </div>
                                    <div class="row">
                                        <div class="col-lg-6">
                                            <base-input alternative=""
                                                        label="Nom"
                                                        placeholder="Nom"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.nom"
                                            />
                                        </div>
                                        <div class="col-lg-6">
                                            <base-input alternative=""
                                                        label="Prénom"
                                                        placeholder="Prénom"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.prenom"
                                            />
                                        </div>
                                    </div>
                                </div>
                                <hr class="my-4" />
                                <!-- Address -->
                                <h6 class="heading-small text-muted mb-4">Information de contact</h6>
                                <div class="pl-lg-4">
                                    <div class="row">
                                        <div class="col-md-12">
                                            <base-input alternative=""
                                                        label="Adresse civile"
                                                        placeholder="adresse"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.addresse"
                                            />
                                        </div>
                                    </div>
                                    <div class="row">
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="commune"
                                                        placeholder="ex: EL-HARRACH"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.commune"
                                            />
                                        </div>
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="Wilaya"
                                                        placeholder="ex: ALGER"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.wilaya"
                                            />
                                        </div>
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="Numéro de téléphone"
                                                        placeholder="ex: 0555778899"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.num"
                                            />
                                        </div>
                                    </div>
                                </div>
                                <hr class="my-4" />
                                <!-- Description -->
                                <h6 class="heading-small text-muted mb-4">Inscrpition</h6>
                                <div class="pl-lg-4">
                                    <div class="row">
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="Promo"
                                                        placeholder="ex: 1CS"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.promo"
                                            />
                                        </div>
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="Section"
                                                        placeholder="ex: C"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.section"
                                            />
                                        </div>
                                        <div class="col-lg-4">
                                            <base-input alternative=""
                                                        label="Groupe"
                                                        placeholder="ex: 08"
                                                        input-classes="form-control-alternative"
                                                        v-model="model.groupe"
                                            />
                                        </div>
                                        <a href="#!" class="btn btn-info">Valider!</a>
                                    </div>
                                </div>
                            </form>
                        </template>
                    </card>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
  export default {
    name: 'user-profile',
    data() {
      return {
        model: {
          matricule: '',
          email: '',
          nom: '',
          prenom: '',
          addresse: '',
          commune: '',
          wilaya: '',
          num: '',
          promo: '',
          section: '',
          groupe: '',
        }
      }
    },
  };
</script>
<style></style>
