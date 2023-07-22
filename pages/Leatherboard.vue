<template>
    <body>
        <h1 id="leatherboard">Leaderboard</h1>
        <table>
          <thead>
            <tr>
              <th>Date & time</th>
              <th>Destroyed asteroids</th>
              <th>Score</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="(data, datetime) in board" :key="datetime">
                <td>{{ formatDateTime(datetime) }}</td>
                <td>{{ data.destroyedAsteroids }}</td>
                <td>{{ data.score }}</td>
            </tr>
          </tbody>
        </table>
    </body>
  </template>
  
  <script setup>
    import titleImg from "assets/title.png"
    </script>

  <script>
  import JSON from '~/score/Leaderboard.json'
  
  export default {
    data() {
        return {
        board: JSON,
        };
    },
    methods: {
        formatDateTime(datetime) {
        return new Date(datetime).toLocaleString();
        },
    },
  };
  </script>
  
<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@200&family=Tektur&display=swap');
    body
    {
        background-color: #010507;
    }
    #leatherboard 
    {
        font-size: 40pt;
    }

    table
    {
        margin-left: auto;
        margin-right: auto;
        color: white;
        text-align: center;
        font-family: Montserrat;
        font-size: 15pt;
    }
    th
    {
        border-bottom: dotted 1px white;
        text-transform: uppercase;
        padding-bottom: 1%;
    }
    td
    {
        padding-top: 1.4%;
    }
  
</style>