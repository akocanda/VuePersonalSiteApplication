<template>
    <b-card-body>
        <b-card-title>Skills</b-card-title>
        <b-card-group deck>
            <b-card no-body header="Technical">
                <b-list-group flush>
                    <b-list-group-item>Vue.js, HTML5, Freemarker, Bootstrap, Javascript</b-list-group-item>
                    <b-list-group-item>Java 8, Spring Boot, Lombok, RabbitMq</b-list-group-item>
                    <b-list-group-item>Karma, Selenium, JUnit5</b-list-group-item>
                    <b-list-group-item>Pivotal Cloud Foundry, Heroku, AppDynamics, Kibana</b-list-group-item>
                    <b-list-group-item>MariaDB, MySql</b-list-group-item>
                    <b-list-group-item>Docker</b-list-group-item>
                </b-list-group>
            </b-card>
            <b-card no-body header="Design and Workplace Methodologies">
                <b-list-group flush>
                    <b-list-group-item>Event Driven Design</b-list-group-item>
                    <b-list-group-item>Test Driven Development</b-list-group-item>
                    <b-list-group-item>Domain Driven Development</b-list-group-item>
                    <b-list-group-item>Microservice Architecture</b-list-group-item>
                    <b-list-group-item>XP (Paired) Programming</b-list-group-item>
                </b-list-group>
            </b-card>
            <b-card no-body header="Check Out Some of My Projects" style="background-color: darkgreen; color: white;">
                <b-list-group>
                    <b-list-group-item href="https://github.com/akocanda/VuePersonalSiteApplication" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                            <h5 class="mb-1">Vue.js Personal Website Application</h5>
                        </div>
                        <p class="mb-1">
                            The site that you are currently on is built on the Vue.js framework
                        </p>
                        <b-form-tags
                                v-model="personalWebsiteTools"
                                placeholder=""
                                size="md"
                                disabled
                        ></b-form-tags>
                    </b-list-group-item>
                    <b-list-group-item href="https://github.com/akocanda/spring-boot" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                            <h5 class="mb-1">Spring Boot Application</h5>
                        </div>
                        <p class="mb-1">
                            Set of tutorials to learn Spring Boot application principles
                        </p>
                        <b-form-tags
                                v-model="springBootTools"
                                placeholder=""
                                size="md"
                                disabled
                        ></b-form-tags>
                    </b-list-group-item>
                </b-list-group>
            </b-card>
        </b-card-group>
    </b-card-body>
</template>

<script>
    export default {
        props: {
        },
        data() {
              return {
                personalWebsiteTools: ['Vue.js', 'bootstrap-vue.js', 'JavaScript', 'CSS', 'Heroku', 'Node.js'],
                springBootTools: ['Spring Boot', 'JUnit5', 'Java 8']
        }
    }};
</script>

<style>
.flex-container {
  display: flex;
  flex-direction: row;
}
.item {
  flex-grow: 2
}
.card-deck {
padding: 0px 20px 20px 20px;
}
.b-form-tags.disabled {
    background-color: none;
}
</style>
