<template>
  <div class="swagger" id="swagger"></div>
</template>

<script>
import SwaggerUI from "swagger-ui";
import "swagger-ui/dist/swagger-ui.css";

export default {
  name: "Swagger",
  mounted() {
    SwaggerUI({
      url: "https://petstore3.swagger.io/api/v3/openapi.json",
      dom_id: "#swagger",
    });
  },
};
</script>