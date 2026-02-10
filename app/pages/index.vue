<template>
  <div>
    <v-row>
      <v-col cols="12" md="3">
        <v-card height="120" color="black">
          <v-card-text>
            <v-row align="center">
              <!-- right column -->
              <v-col>
                <v-icon size="80">mdi-account</v-icon>
              </v-col>

              <!-- left column -->
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h5">Student</v-col>
                  <v-col cols="12" class="text-right text-h3">120</v-col>

                </v-row>
              </v-col>

            </v-row>
          </v-card-text>


        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" color="red">
          <v-card-text>
            <v-row align="center">
              <!-- right column -->
              <v-col>
                <v-icon size="80">mdi-home</v-icon>
              </v-col>

              <!-- left column -->
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h5">Student</v-col>
                  <v-col cols="12" class="text-right text-h3">120</v-col>

                </v-row>
              </v-col>

            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" color="pink">
          <v-card-text>
            <v-row align="center">
              <!-- right column -->
              <v-col>
                <v-icon size="80">mdi-cash</v-icon>
              </v-col>

              <!-- left column -->
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h5">Student</v-col>
                  <v-col cols="12" class="text-right text-h3">120</v-col>

                </v-row>
              </v-col>

            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" color="blue">
          <v-card-text>
            <v-row align="center">
              <!-- right column -->
              <v-col>
                <v-icon size="80">mdi-human</v-icon>
              </v-col>

              <!-- left column -->
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h5">Student</v-col>
                  <v-col cols="12" class="text-right text-h3">120</v-col>

                </v-row>
              </v-col>

            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="8">
    <v-card  height="400" color="#EEEEEE">
      <v-table density="compact">
    <thead>
      <tr>
        <th class="text-left">
          Name
        </th>
        <th class="text-left">
          Calories
        </th>
      </tr>
    </thead>
    <tbody>
      <tr
        v-for="item in desserts"
        :key="item.name"
      >
        <td>{{ item.name }}</td>
        <td>{{ item.calories }}</td>
      </tr>
    </tbody>
  </v-table>
    </v-card>
    </v-col>
    
    <v-row>
      <v-col>

     <v-col cols="12" md="12">
    <v-card  height="140" color="#EEEEEE">
      
    </v-card>
    </v-col>

    <v-col cols="12" md="12">
    <v-card  height="140" color="#EEEEEE"></v-card>
    </v-col>

    <v-col cols="12" md="12">
    <v-card  height="140" color="#EEEEEE"></v-card>
    </v-col>
    
    </v-col>
   </v-row>

    </v-row>

  
    

    
  </div>
</template>

<script setup>
import { ref } from 'vue'

  const desserts = ref([
    {
      name: 'Frozen Yogurt',
      calories: 159,
    },
    {
      name: 'Ice cream sandwich',
      calories: 237,
    },
    {
      name: 'Eclair',
      calories: 262,
    },
    {
      name: 'Cupcake',
      calories: 305,
    },
    {
      name: 'Gingerbread',
      calories: 356,
    },
    {
      name: 'Jelly bean',
      calories: 375,
    },
    {
      name: 'Lollipop',
      calories: 392,
    },
    {
      name: 'Honeycomb',
      calories: 408,
    },
    {
      name: 'Donut',
      calories: 452,
    },
    {
      name: 'KitKat',
      calories: 518,
    },
  ])


</script>

<style>

</style>