<template>
  <div class="">
    <div class="container prod-header">
      <b-jumbotron>
        <template v-slot:header>机械行业解决方案</template>

        <template v-slot:lead>
          This is a simple hero unit, a simple jumbotron-style component for
          calling extra attention to featured content or information.
        </template>

        <hr class="my-4" />

        <p>
          It uses utility classes for typography and spacing to space content
          out within the larger container.
        </p>

        <b-button variant="primary" href="#">Do Something</b-button>
        <b-button variant="success" href="#">Do Something Else</b-button>
      </b-jumbotron>
    </div>

    <div class="container prod">
      <div>
        <p>适用于：细分行业</p>
        <b-container fluid class="p-4">
          <b-row>
            <b-col>
              <b-img
                thumbnail
                fluid
                src="https://picsum.photos/250/250/?image=54"
                alt="Image 1"
              ></b-img>
            </b-col>
            <b-col>
              <b-img
                thumbnail
                fluid
                src="https://picsum.photos/250/250/?image=58"
                alt="Image 2"
              ></b-img>
            </b-col>
            <b-col>
              <b-img
                thumbnail
                fluid
                src="https://picsum.photos/250/250/?image=59"
                alt="Image 3"
              ></b-img>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <article>
        <section>
          <p>行业特点</p>
          <ul>
            <li>订单以多品种小批量为主，存在汽配等领域标准零件大批量生产</li>
            <li>生产过程存在项目制造/单件制造</li>
            <li>
              产品工艺复杂多变，每个产品工艺各不相同，对工艺流程执行监控要求高
            </li>
            <li>部分工序需要外协加工，产能不足时需要外协加工</li>
            <li>生产设备昂贵，制造成本高</li>
          </ul>

          <b-img
            src="~assets/reallink/images/208669af854a9c882a155a847349ea5c.jpg"
            rounded
            center
            fluid
            my-5
            alt="Responsive image"
            style="width:80%"
          ></b-img>
        </section>
        <section>
          <p>行业现状</p>
          <ul>
            <li>订单准时交货率低，订单进度不能及时掌控</li>
            <li>
              外协加工进度失控及不良率高，影响订单工序计划，易造成交期延期。
            </li>
            <li>
              加工过程返工及报废率高，生产过程因图纸和操作规范问题导致不良较多
            </li>
            <li>图纸、SOP手工管理、人工变更管理难度大、效率低、易出错。</li>
            <li>制造过程品控与质量追溯不健全</li>
            <li>设备综合利用率低，产能效率低，制造成本高。</li>
            <li>
              生产设备品牌型号多，部分设备无接口协议，无设备运行状态监控。
            </li>
          </ul>

          <b-img
            src="~assets/reallink/images/c2c6d4edefcef10e46622532a209334b.png"
            rounded
            center
            fluid
            my-5
            alt="Responsive image"
            style="width:80%"
          ></b-img>
        </section>

        <section>
          <p>行业需求</p>
          <ul>
            <li>
              基础数据量大、订单多、数据变更频繁，需要与ERP数据共享、业务协同联控。
            </li>
            <li>
              物料形态多样、余料多不易识别利用，需要系统管理、收发物料条码自动识别
            </li>
            <li>订单作业计划排程、产能负荷实时动态统计，合理排产提升设备OEE</li>
            <li>
              作业计划与生产派工协同，直接派工到员工工位，生产执行实时监控及调度调整。
            </li>
            <li>
              订单生产进度（含外协工序）实时掌控，支持销售跟单查生产进度。
            </li>
            <li>生产加工执行动态数据实时采集，精准掌握生产状态。</li>
            <li>
              检验工序流程控制，检验数据在线采集，降低人为失误导致的错误。
            </li>
            <li>
              不良原因实时统计预警，不良处理系统流程管理，对不良责任人工、返工工时等记录，便于事后分析改善。
            </li>
            <li>关注异常发生与处理，及时处理异常，减少停工等待</li>
            <li>设备状态实时监控，加工效率实时自动统计。</li>
            <li>图纸文件在线查看，无纸化应用</li>
          </ul>
          <b-img
            src="~assets/reallink/images/c2c6d4edefcef10e46622532a209334b.png"
            rounded
            center
            fluid
            my-5
            alt="Responsive image"
            style="width:80%"
          ></b-img>
        </section>

        1. 作业计划与生产执行协同，提升产能效率。 >
        APS生产计划排程系统与ERP集成，根据生产订单交期、工艺路线、工序产能、及在制订单产能需求等信息，辅助人工计划排程，并实现排程结果派工和执行数据实时跟踪分析，提升准时交货率、提高产能、降低在制成本。
        <img
          src="~assets/reallink/images/891b14c1f4d1874b077ec4f241a05945.png"
          alt=""
        />
        1. 生产执行数据采集 >
        MES生产执行系统，采用最新信息技术和网络技术，实现业务流程协同、与底层自动化设备的PLC系统集成打通，对车间人、机、料、法、环、质等生产要素进行全面管控，实现企业精益制造和数字化管理。
        <img
          src="~assets/reallink/images/05635c6f850eb73b0b1c6b9cc151641f.png"
          alt=""
        />
        1. 在线检验、任务驱动、规范管理 >
        QMS质检系统，通过与ERP、WMS、MES业务流程协同，待检任务自动推送，移动PAD在线检验，现场查阅操作规范说明、现场查阅规格说明书、图纸文件、现场拍照取证、及录入检验参数，提高检验规范、提高质检效率。
        <img
          src="~assets/reallink/images/3c5945b4a68459f0aa697a8c80dd9d24.png"
          alt=""
        />
        1. 数字化生产、可视化管理 >
        从计划任务、备料、检验、产线生产统计、质检统计、生产状态监控、生产进度监控等全方位对生产过程进行实时监控，问题及时处理。
        <img
          src="~assets/reallink/images/0485899424f1418101f52cfe35f2afd9.png"
          alt="Image"
        />
        1. 方案收益
        <img
          src="~assets/reallink/images/dec7a4046a32e66e3ddbb6220954b5f1.jpg"
          alt="Image"
        />
      </article>
    </div>
  </div>
</template>

<script>
export default {}
</script>
