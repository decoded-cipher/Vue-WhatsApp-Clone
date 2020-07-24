<template>
  <div>
    <ChatHeader />
    <div v-for="(chat, i) in chats" :key="i">
      <router-link to="/messages">
        <ChatLists :data="chat" />
      </router-link>
    </div>
  </div>
</template>

<script>
  import ChatHeader from "../components/chats/Header";
  import ChatLists from "../components/chats/Lists";
  export default {
    name: "Chats",
    components: {
      ChatHeader,
      ChatLists
    },
    data() {
      return {
        chats: [{
            image: "https://scontent.fcok1-1.fna.fbcdn.net/v/t31.0-8/21167183_647228462147917_6835871421253726589_o.jpg?_nc_cat=108&_nc_sid=174925&_nc_ohc=K2Ju1V-hAhQAX-gei58&_nc_ht=scontent.fcok1-1.fna&oh=d988b4fc8f12926c7e493779a0cd092e&oe=5F4183D2",
            name: "Bharath BCA",
            message: "Yeah, I think we must have to...",
            time: "11:45 AM",
            count: 3
          },
          {
            image: "https://scontent.fcok1-1.fna.fbcdn.net/v/t1.0-9/51623544_2156240734687879_4688845161734602752_o.jpg?_nc_cat=105&_nc_sid=09cbfe&_nc_ohc=n8kpMXSuNi0AX93uK0h&_nc_ht=scontent.fcok1-1.fna&oh=c735e4849972bb3651c9934725354501&oe=5F408987",
            name: "Ashwin LFVN",
            message: "Asus VivoBook 15 Core i5 8th Gen - ",
            time: "11:39 AM",
            count: 1
          },
          {
            image: "https://avatars3.githubusercontent.com/u/971925?s=400&v=4",
            name: "Jithin Chettan, Inovus",
            message: "Try Ghost CMS",
            time: "Yesterday",
            count: 0
          },
          {
            image: "https://scontent.fcok1-1.fna.fbcdn.net/v/t1.0-9/85105680_1080874525597808_1573310043091107840_n.jpg?_nc_cat=106&_nc_sid=e3f864&_nc_ohc=Bg_qUvHUwrcAX_IUX2y&_nc_ht=scontent.fcok1-1.fna&oh=4241641a7ef05a6987202b20d702fa98&oe=5F413BD6",
            name: "Laya Inovus",
            message: "0:07",
            time: "Yesterday",
            count: 0
          },
          {
            image: "https://scontent.fcok1-1.fna.fbcdn.net/v/t31.0-8/12525576_1691777821088307_2174139030434778545_o.png?_nc_cat=102&_nc_sid=09cbfe&_nc_ohc=yfS-fiBMqbAAX-vcY8j&_nc_ht=scontent.fcok1-1.fna&oh=de4c8c88b78b11c97ff65605931036c2&oe=5F40B3F8",
            name: "Inovus Labs Official",
            message: "Laya: Sounds good!",
            time: "7/22/20",
            count: 0
          },
          {
            image: "https://cdn.idsitnetwork.net/wp-content/uploads/sites/27/2019/01/flower-shop-fields-of-romance-148245.jpg",
            name: "Binny Miss",
            message: "Include the Character Recogn...",
            time: "7/22/20",
            count: 1
          },
          {
            image: "https://avatars3.githubusercontent.com/u/971925?s=400&v=4",
            name: "Freddy Chettan, Inovus",
            message: "0:43",
            time: "7/22/20",
            count: 0
          },
          {
            image: "https://media-exp1.licdn.com/dms/image/C5103AQHVodNd4yYrBw/profile-displayphoto-shrink_800_800/0?e=1600905600&v=beta&t=zDiQtzikkYbtc0sMc6VDb6Imi87r-cHaj8GAd0-m_aU",
            name: "Thomas BCA, Inovus",
            message: "Image",
            time: "7/21/20",
            count: 0
          }
        ]
      };
    }
  };
</script>