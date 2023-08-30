<template>
  <view>
    <tantan :list="list" @="change" @Image="clickImage"></tantan>
  </view>
</template>

<script>
import tantan from '@/components/dgex-tantan/dgex-tantan.vue'
export default {
  components: {
    tantan
  },
  data() {
    return {
      list: []
    }
  },
  mounted() {
    const arr = []
    /* 测试数据*/
    const tu = [
      'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
      'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
      'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
      'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500',
	  'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fpic1.win4000.com%2Fmobile%2F2020-06-19%2F5eec5f30c7a71.jpg&refer=http%3A%2F%2Fpic1.win4000.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1662573014&t=e46c2e2622713d2a5c4d2a325ab1f08d'
    ]
    for (let index = 0; index < 10; index++) {
      const n = Math.floor(Math.random() * (tu.length - 1))
      let data = {
        image: tu[n],
        title: '你好',
        desc: n + 500 + 'm ' + '30分钟前活跃',
        tags: ['射手座']
      }
      arr.push(data)
    }
    this.list = arr
  },
  methods: {
    change(data) {
		
		console.log(data);
      // 判断倒数
      if (data.currentIndex > this.list.length - 5) {
        // 模拟一下最加数据
        const tu = [
          'https://nimg.ws.126.net/?url=http%3A%2F%2Fdingyue.ws.126.net%2F2021%2F0704%2Fc7a27a1ej00qvpu700019c000hs00vlc.jpg&thumbnail=660x2147483647&quality=80&type=jpg',
          'https://nimg.ws.126.net/?url=http%3A%2F%2Fdingyue.ws.126.net%2F2021%2F0704%2F9f81e6aaj00qvpu70001xc000hs00vmc.jpg&thumbnail=660x2147483647&quality=80&type=jpg',
          'https://nimg.ws.126.net/?url=http%3A%2F%2Fdingyue.ws.126.net%2F2021%2F0704%2F55bf2cb3j00qvpu70002cc000hs012jc.jpg&thumbnail=660x2147483647&quality=80&type=jpg',
          'https://nimg.ws.126.net/?url=http%3A%2F%2Fdingyue.ws.126.net%2F2021%2F0704%2F2017725bj00qvpu70001jc000hs00zxc.jpg&thumbnail=660x2147483647&quality=80&type=jpg'
        ]
        for (let index = 0; index < 10; index++) {
          const n = Math.floor(Math.random() * (tu.length - 1))
          let newdata = {
            image: tu[n],
            title: '你好',
            desc: n + 500 + 'm ' + '30分钟前活跃',
            tags: ['射手座']
          }
          this.list.push(newdata)
        }
      }
    },
    clickImage(data) {
      console.log(data);
    }
  }
}
</script>