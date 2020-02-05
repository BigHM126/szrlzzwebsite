<template>
  <div>
    <div class="container-fluid">
      <div class="container-fluid bg-light">
        <section class="container py-3">
          <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="2500"
            @sliding-start="onSlideStart"
            @sliding-end="onSlideEnd"
            fade
            controls
            indicators
            background="#ababab"
            img-width="1024"
            img-height="420"
            style="text-shadow: 1px 1px 2px #333;"
          >
            <!-- Text slides with image -->
            <!--             <b-carousel-slide
              v-for="(item, index) in bannerCarousel"
              :key="index"
            >
              <template v-slot:img>
                <b-img
                  :src="'~assets/reallink/images/slide' + index + 1 + '.png'"
                  class="d-block img-fluid w-100"
                  width="1024"
                  height="420"
                  alt="image slot"
                ></b-img>
              </template>
            </b-carousel-slide> -->
            <b-carousel-slide
              img-src="~assets/reallink/images/slide1.png"
              class="text-left"
            ></b-carousel-slide>
            <b-carousel-slide
              img-src="~assets/reallink/images/slide2.png"
              class="text-left"
            ></b-carousel-slide>
            <b-carousel-slide
              img-src="~assets/reallink/images/slide3.png"
              class="text-left"
            ></b-carousel-slide>
          </b-carousel>
        </section>
      </div>
      <section class="container">
        <div class="row m-2 justify-content-between">
          <h5>
            行业方案<b-badge pill size="sm" variant="danger" class="mx-3"
              >热门推荐</b-badge
            >
          </h5>
          <p class="text-muted">
            <strong
              ><em
                >一套“快速应用、操作简便、高效运维”的智能工厂软硬件综合方案</em
              ></strong
            >
          </p>
          <b-link class="pl-5">查阅所有</b-link>
          <!-- <b-button size="sm" class="mb-2" variant="light">
            <span>了解更多</span>
             <b-icon icon="three-dots"></b-icon>
          </b-button> -->
        </div>
        <div class="row">
          <div class="col-md-6">
            <b-card
              title="Card Title"
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="article"
              class="mb-2"
            >
              <b-card-text>
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </b-card-text>
              <div class="d-flex justify-content-between">
                <p>
                  适用于：
                  <mark><strong>机加零件</strong></mark
                  >\<mark><strong>精密设备</strong></mark
                  >等细分行业
                </p>
                <b-button href="#" variant="primary">点击详情</b-button>
              </div>
            </b-card>
          </div>
          <div class="col-md-6">
            <b-card
              title="Card Title"
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="article"
              class="mb-2"
            >
              <b-card-text>
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </b-card-text>
              <div class="d-flex justify-content-between">
                <p>
                  适用于：
                  <mark><strong>机加零件</strong></mark
                  >\<mark><strong>精密设备</strong></mark
                  >等细分行业
                </p>
                <b-button href="#" variant="primary">点击详情</b-button>
              </div>
            </b-card>
          </div>
        </div>
      </section>

      <section class="jumbotron text-center bg-light">
        <div class="container">
          <h1>在线产品</h1>
          <p class="lead text-muted">
            Something short and leading about the collection below—its contents,
            the creator, etc. Make it short and sweet, but not too short so
            folks don’t simply skip over it entirely.
          </p>
        </div>
      </section>
      <section class="container">
        <div class="row">
          <div v-for="(item, index) in 3" :key="index" class="col-md-4">
            <b-card
              no-body
              img-src="https://placekitten.com/380/200"
              img-alt="Image"
              img-top
            >
              <b-card-body>
                <b-card-title>MES-制造执行系统</b-card-title>
                <b-card-text>
                  Some quick example text to build on the card title and make up
                  the bulk of the card's content.
                </b-card-text>
              </b-card-body>

              <b-list-group flush>
                <b-list-group-item
                  ><b-icon
                    icon="award"
                    class="rounded-circle bg-danger"
                    variant="light"
                  ></b-icon
                  ><span class="mx-2">实时查询工序进度</span></b-list-group-item
                >
                <b-list-group-item
                  ><b-icon
                    icon="award"
                    class="rounded-circle bg-danger"
                    variant="light"
                  ></b-icon
                  ><span class="mx-2">及时了解现场状态</span></b-list-group-item
                >
                <b-list-group-item
                  ><b-icon
                    icon="award"
                    class="rounded-circle bg-danger"
                    variant="light"
                  ></b-icon
                  ><span class="mx-2"
                    >报告和分析异常原因</span
                  ></b-list-group-item
                >
              </b-list-group>

              <b-card-body class="right">
                <a href="#" class="card-link">了解详情</a>
                <a href="#" class="card-link">产品文档</a>
              </b-card-body>
            </b-card>
          </div>
        </div>
      </section>
      <section class="jumbotron text-center bg-light">
        <div class="container">
          <h1>客户案例</h1>
          <p class="lead text-muted">
            Something short and leading about the collection below—its contents,
            the creator, etc. Make it short and sweet, but not too short so
            folks don’t simply skip over it entirely.
          </p>
          <blockquote class="blockquote text-center ">
            <p class="mb-0">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
              posuere erat a ante.
            </p>
            <footer class="blockquote-footer">
              Someone famous in <cite title="Source Title">Source Title</cite>
            </footer>
          </blockquote>
          <div class="row m-3">
            <div class="col-lg-8">
              <video width="100%" height="auto" controls>
                <source src="/reallink/media/office.mp4" type="video/mp4" />
                您的浏览器不支持Video标签。
              </video>
            </div>
            <div class="col-lg-4">
              <h4>案例视频||科瑞技术</h4>
              <p class="lead">
                高端自动化装备定制化企业，其业务覆盖全球7个国家，11家实体生产企业。
              </p>
              <ul>
                <li>能长期满足企业的稳定发展</li>
                <li>能承受当前业务规模的负载能力</li>
                <li>有技术实力和大企业支持</li>
                <li>符合SP95行业化标准、可扩展</li>
                <li>配合企业做一定的个性化定制</li>
              </ul>
            </div>
          </div>
          <div class="row m-3">
            <b-card
              img-src="https://placekitten.com/300/300"
              img-alt="Card image"
              img-left
              class="mb-3"
            >
              <b-card-text>
                <footer class="blockquote text-center">
                  <p class="mb-0">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    Integer posuere erat a ante.
                  </p>
                  <footer class="blockquote-footer">
                    Someone famous in
                    <cite title="Source Title">Source Title</cite>
                  </footer>
                </footer>
              </b-card-text>
            </b-card>

            <blockquote class="blockquote text-center ">
              <p class="mb-0">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
                posuere erat a ante.
              </p>
              <footer class="blockquote-footer">
                Someone famous in <cite title="Source Title">Source Title</cite>
              </footer>
            </blockquote>
          </div>
        </div>
      </section>
      <section class="jumbotron text-center bg-light">
        <div class="container">
          <h1>生态联盟</h1>
          <p class="lead text-muted">
            Something short and leading about the collection below—its contents,
            the creator, etc. Make it short and sweet, but not too short so
            folks don’t simply skip over it entirely.
          </p>
        </div>

        <h2>长期战略合作伙伴</h2>
        <div class="row-flex m-4 d-flex justify-content-center">
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=58"
            alt="用友网络"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
        </div>
        <h2>钻石级合作伙伴</h2>
        <div class="row-flex m-4 d-flex justify-content-center">
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=58"
            alt="用友网络"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
        </div>
        <h2>金牌/银牌合作伙伴</h2>
        <div class="row m-4 justify-content-center">
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=58"
            alt="用友网络"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=58"
            alt="用友网络"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=58"
            alt="用友网络"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
          <b-img
            thumbnail
            fluid
            src="https://picsum.photos/250/250/?image=59"
            alt="科瑞技术"
            class="mx-3"
          ></b-img>
        </div>
        <h2>技术合作伙伴</h2>
        <div class="row-flex m-4 d-flex justify-content-center"></div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      slide: 0,
      sliding: null,
      bannerCarousel: [
        {
          caption: '',
          text: '',
          imgSrc: '~assets/reallink/images/slide1.png'
        },
        {
          caption: '',
          text: '',
          imgSrc: '~assets/reallink/images/slide2.png'
        },
        {
          caption: '',
          text: '',
          imgSrc: '~assets/reallink/images/slide3.png'
        }
      ]
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    }
  }
}
</script>

<style></style>
