<template>
  <div id="app" class="container">
    <TableComponent title="Desarrolladores" :users="dev_users" :stylecomp="style1" />
    <TableComponent title="Testers" :users="test_users" :stylecomp="style2" />
    <TableComponent title="Administradores" :users="prod_users" :stylecomp="style3" />
  </div>
</template>

<script>
import TableComponent from "./components/TableComponent.vue";

export default {
  name: "App",
  data() {
    return {
      style1: {
        background: "#FEEBC8",
        border: "1px solid #ED8936",
        color: "#9C4221",
      },
      style2: {
        background: "#2c5282",
        border: "1px solid #3182ce",
        color: "#ebf8ff",
      },
      style3: {
        background: "#065666",
        border: "1px solid #00A3C4",
        color: "#EDFDFD",
      },
      prod_users: [
        {
          id: 1,
          username: "jbreddy0",
          email: "gkingcott0@amazon.co.uk",
          password: "b315c7464fd2964822f74d97814f3aa0",
          create_at: "3/13/2022",
          ip_address: "219.80.54.171",
          bloked: true,
        },
        {
          id: 2,
          username: "njessep1",
          email: "fedgcombe1@walmart.com",
          password: "700de9c066f56800ac73c59b6d6ae1c6",
          create_at: "10/3/2022",
          ip_address: "202.24.23.233",
          bloked: false,
        },
        {
          id: 3,
          username: "wlukasik2",
          email: "rcaban2@imdb.com",
          password: "1ecfc3b9e9cfe53d4c31e4b03addf7a8",
          create_at: "12/19/2021",
          ip_address: "44.183.134.132",
          bloked: true,
        },
        {
          id: 4,
          username: "cconnochie3",
          email: "rwealthall3@comcast.net",
          password: "b27831d715cd9891262451478ce3e507",
          create_at: "1/21/2022",
          ip_address: "30.239.230.114",
          bloked: false,
        },
        {
          id: 5,
          username: "mspillard4",
          email: "mblackeby4@aol.com",
          password: "c9cb281d01ce7091778b85b60f0bd9a5",
          create_at: "7/6/2022",
          ip_address: "170.149.172.65",
          bloked: false,
        },
        {
          id: 6,
          username: "mtuny5",
          email: "ewhinney5@theglobeandmail.com",
          password: "4db8635f106607b423b68ab1cb2d68bd",
          create_at: "8/18/2022",
          ip_address: "117.125.163.28",
          bloked: false,
        },
        {
          id: 7,
          username: "dlawland6",
          email: "ddegiorgio6@marriott.com",
          password: "232cb758d093f3adf68e36f4501f6c46",
          create_at: "10/22/2022",
          ip_address: "117.34.78.253",
          bloked: true,
        },
        {
          id: 8,
          username: "apersicke7",
          email: "ateligin7@ycombinator.com",
          password: "1d528e4c79d28291762e77d945048f4a",
          create_at: "6/27/2022",
          ip_address: "134.216.50.203",
          bloked: false,
        },
        {
          id: 9,
          username: "ccoarser8",
          email: "sminnette8@aol.com",
          password: "07396d1fe5f5123231051ab53cc4d5c8",
          create_at: "12/13/2021",
          ip_address: "152.232.96.210",
          bloked: true,
        },
        {
          id: 10,
          username: "lsnap9",
          email: "jmenis9@moonfruit.com",
          password: "faae4096ee5508f391fe5b9fd8f31673",
          create_at: "9/6/2022",
          ip_address: "87.163.52.223",
          bloked: true,
        },
      ],
      test_users: [
        {
          id: 11,
          username: "ljouhana",
          email: "wwalchera@imgur.com",
          password: "83a8d1c31d9c48b18abc138da4582073",
          create_at: "4/6/2022",
          ip_address: "210.164.199.152",
          bloked: true,
        },
        {
          id: 12,
          username: "jrowettb",
          email: "kphillotb@woothemes.com",
          password: "c9c17c0cde038ebddf0d3a5ab3cf20f6",
          create_at: "10/7/2022",
          ip_address: "147.2.64.248",
          bloked: true,
        },
        {
          id: 13,
          username: "cpottiec",
          email: "ajeggoc@eepurl.com",
          password: "f7319c268e8a10a54b291853d24db233",
          create_at: "8/7/2022",
          ip_address: "218.60.40.40",
          bloked: false,
        },
        {
          id: 14,
          username: "jzuted",
          email: "kcuddyd@ezinearticles.com",
          password: "3eab3c6abca515059a9112b2d2b78f72",
          create_at: "3/1/2022",
          ip_address: "154.63.131.215",
          bloked: false,
        },
        {
          id: 15,
          username: "creamese",
          email: "plamminge@360.cn",
          password: "42a8578529becb1df68a4287213ca5e7",
          create_at: "1/21/2022",
          ip_address: "215.54.99.119",
          bloked: false,
        },
        {
          id: 16,
          username: "bgeryf",
          email: "cdiemf@list-manage.com",
          password: "a494110f01a5bbcef2ad6b1b8af2d94b",
          create_at: "11/16/2022",
          ip_address: "155.136.252.146",
          bloked: false,
        },
        {
          id: 17,
          username: "honiong",
          email: "lknivettg@bandcamp.com",
          password: "6726fcd92e5cba75d5c2ae78bbe57b49",
          create_at: "12/23/2021",
          ip_address: "80.30.178.190",
          bloked: true,
        },
        {
          id: 18,
          username: "omaccartanh",
          email: "mchappelh@nasa.gov",
          password: "c0231f6f6c9f8b68cf8c476f60a39a9e",
          create_at: "12/25/2021",
          ip_address: "228.195.141.85",
          bloked: false,
        },
        {
          id: 19,
          username: "wpharoahi",
          email: "shoveei@edublogs.org",
          password: "111e5b3c41237778646db565fffbe8e3",
          create_at: "2/10/2022",
          ip_address: "157.196.208.87",
          bloked: true,
        },
        {
          id: 20,
          username: "jahlfj",
          email: "dfreemantlej@unc.edu",
          password: "79472acea07717b803d722942d8fcdf5",
          create_at: "7/2/2022",
          ip_address: "108.217.114.48",
          bloked: true,
        },
      ],
      dev_users: [
        {
          id: 21,
          username: "dlyallk",
          email: "rchavrink@home.pl",
          password: "2b09fe069604b72bccec6bf11c21e139",
          create_at: "6/4/2022",
          ip_address: "142.76.120.130",
          bloked: true,
        },
        {
          id: 22,
          username: "abestel",
          email: "imaylaml@linkedin.com",
          password: "b87d515a61723fddbc032c33b9d0ca04",
          create_at: "1/9/2022",
          ip_address: "252.204.24.48",
          bloked: false,
        },
        {
          id: 23,
          username: "jkeenm",
          email: "abaldersonm@tuttocitta.it",
          password: "d34f9e3edf093ee0cfbf6b6c7c04d700",
          create_at: "3/23/2022",
          ip_address: "17.216.167.83",
          bloked: false,
        },
        {
          id: 24,
          username: "dfrettern",
          email: "pradbournn@yellowbook.com",
          password: "1e79d832f01a29525cf968e6d0b63292",
          create_at: "5/3/2022",
          ip_address: "180.45.103.177",
          bloked: true,
        },
        {
          id: 25,
          username: "srapaporto",
          email: "lthorogoodo@gmpg.org",
          password: "2ed03767a70d972cb5098a63831d080c",
          create_at: "4/8/2022",
          ip_address: "229.8.244.42",
          bloked: false,
        },
        {
          id: 26,
          username: "sminterp",
          email: "vdewerp@yolasite.com",
          password: "117fe047a6416b60c14e6326bde72cae",
          create_at: "10/25/2022",
          ip_address: "186.225.76.60",
          bloked: true,
        },
        {
          id: 27,
          username: "alanstonq",
          email: "hokieranq@weebly.com",
          password: "b1cdb099101215f2fa129ecb5e9366c6",
          create_at: "12/11/2021",
          ip_address: "88.123.134.243",
          bloked: false,
        },
        {
          id: 28,
          username: "hcaygillr",
          email: "ksoppettr@icq.com",
          password: "3c85603a1a8b1f3eb955cd996db6a8d9",
          create_at: "12/21/2021",
          ip_address: "202.84.110.30",
          bloked: true,
        },
        {
          id: 29,
          username: "talderss",
          email: "skynmans@hugedomains.com",
          password: "5cc502acccf96dcb9745bbdf132dfe03",
          create_at: "5/28/2022",
          ip_address: "172.129.147.86",
          bloked: false,
        },
        {
          id: 30,
          username: "mpepperdt",
          email: "mhoulstont@samsung.com",
          password: "bd95627e1da4a74c6be26014abdc4d3e",
          create_at: "9/28/2022",
          ip_address: "158.213.230.196",
          bloked: true,
        },
      ],
    };
  },
  components: {
    TableComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
