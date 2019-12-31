<template>
    <div>
        <base-header type="gradient-success" class="pb-6 pb-8 pt-5 pt-md-8">
            <!-- Card stats -->
            <div class="row">
                <div class="col-xl-3 col-lg-6">
                    <stats-card title="Promo 1CP"
                                type="gradient-red"
                                sub-title="267"
                                icon="ni ni-active-40"
                                class="mb-4 mb-xl-0">

                        <template slot="footer">
                            <span class="text-success mr-2"><i class="fa fa-arrow-up"></i> 28.58%</span>
                            <span class="text-nowrap">Du total des étudiants <br>(mise à part la promo 3CS)</span>
                        </template>
                    </stats-card>
                </div>
                <div class="col-xl-3 col-lg-6">
                    <stats-card title="Promo 2CP"
                                type="gradient-orange"
                                sub-title="223"
                                icon="ni ni-chart-pie-35"
                                class="mb-4 mb-xl-0">

                        <template slot="footer">
                            <span class="text-success mr-2"><i class="fa fa-arrow-up"></i> 23.87%</span>
                            <span class="text-nowrap">Du total des étudiants <br>(mise à part la promo 3CS).</span>
                        </template>
                    </stats-card>
                </div>
                <div class="col-xl-3 col-lg-6">
                    <stats-card title="Promo 1CS"
                                type="gradient-green"
                                sub-title="254"
                                icon="ni ni-money-coins"
                                class="mb-4 mb-xl-0">

                        <template slot="footer">
                            <span class="text-danger mr-2"><i class="fa fa-arrow-down"></i> 27.19%</span>
                            <span class="text-nowrap">Du total des étudiants <br>(mise à part la promo 3CS)</span>
                        </template>
                    </stats-card>

                </div>
                <div class="col-xl-3 col-lg-6">
                    <stats-card title="Promo 2cs"
                                type="gradient-info"
                                sub-title="190"
                                icon="ni ni-chart-bar-32"
                                class="mb-4 mb-xl-0">

                        <template slot="footer">
                            <span class="text-success mr-2"><i class="fa fa-arrow-up"></i> 20.34%</span>
                            <span class="text-nowrap">Du total des étudiants <br>(mise à part la promo 3CS)</span>
                        </template>
                    </stats-card>
                </div>
                
            </div>
        </base-header>

        <div class="container-fluid mt--7">
            <div class="row">
                <div class="col">
                    <projects-table title="Liste des étudiants"></projects-table>
                </div>
            </div>
            <!-- <div class="row mt-5"> 
                <div class="col">
                    <projects-table type="dark" title="Dark Table"></projects-table>
                </div>
            </div> -->
        </div>

    </div>
</template>
<script>
  import ProjectsTable from './Tables/ProjectsTable'
  export default {
    name: 'tables',
    components: {
      ProjectsTable
    }
  };
</script>
<style></style>
