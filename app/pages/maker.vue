<template>
    <div id="tab-wrapper">
        <div id="tab-items">
            <div class="tab-item act" @click="tabclick(0)" id="tab0">
                <div>바디</div>
            </div>
            <div class="tab-item" @click="tabclick(1)" id="tab1">
                <div>눈썹</div>
            </div>
            <div class="tab-item" @click="tabclick(2)" id="tab2">
                <div>왼눈</div>
            </div>
            <div class="tab-item" @click="tabclick(3)" id="tab3">
                <div>오른눈</div>
            </div>
            <div class="tab-item" @click="tabclick(4)" id="tab4">
                <div>입</div>
            </div>
            <div class="tab-item" @click="tabclick(5)" id="tab5">
                <div>홍조</div>
            </div>
            <div class="tab-item" @click="tabclick(6)" id="tab6">
                <div>뒷머리</div>
            </div>
            <div class="tab-item" @click="tabclick(7)" id="tab7">
                <div>앞머리</div>
            </div>
            <div class="tab-item" @click="tabclick(8)" id="tab8">
                <div>옆머리L</div>
            </div>
            <div class="tab-item" @click="tabclick(9)" id="tab9">
                <div>옆머리R</div>
            </div>
            <div class="tab-item" @click="tabclick(10)" id="tab10">
                <div>머리+</div>
            </div>
            <div class="tab-item" @click="tabclick(13)" id="tab13">
                <div>상의</div>
            </div>
            <div class="tab-item" @click="tabclick(14)" id="tab14">
                <div>하의</div>
            </div>
            <div class="tab-item" @click="tabclick(15)" id="tab15">
                <div>겉옷</div>
            </div>
            <div class="tab-item" @click="tabclick(16)" id="tab16">
                <div>양말</div>
            </div>
            <div class="tab-item" @click="tabclick(17)" id="tab17">
                <div>신발</div>
            </div>
        </div>
        <div id="content-items">
            <div class="content-item act" id="content0">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color0"/>
                    </div>
                    <div class="item">
                        기본 몸통
                    </div>
                </div>
            </div>
            <div class="content-item" id="content1">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color1"/>
                    </div>
                    <div class="item">
                        일자눈썹
                    </div>
                </div>
            </div>
            <div class="content-item" id="content2">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color2"/>
                    </div>
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color2_1"/>
                    </div>
                    <div class="item">
                        동그란눈
                    </div>
                </div>
            </div>
            <div class="content-item" id="content3">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color3"/>
                    </div>
                    <div class="item">
                        동그란눈
                    </div>
                </div>
            </div>
            <div class="content-item" id="content4">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color4"/>
                    </div>
                    <div class="item">
                        고양이입
                    </div>
                </div>
            </div>
            <div class="content-item" id="content5">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color5"/>
                    </div>
                    <div class="item">
                        홍조
                    </div>
                </div>
            </div>
            <div class="content-item" id="content6">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color6"/>
                    </div>
                    <div class="item">
                        기본 머리
                    </div>
                </div>
            </div>
            <div class="content-item" id="content7">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color6"/>
                    </div>
                    <div class="item">
                        일자 앞머리
                    </div>
                </div>
            </div>
            <div class="content-item" id="content8">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color6"/>
                    </div>
                    <div class="item">
                        긴 옆머리
                    </div>
                </div>
            </div>
            <div class="content-item" id="content9">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color6"/>
                    </div>
                    <div class="item">
                        긴 옆머리
                    </div>
                </div>
            </div>
            <div class="content-item" id="content10">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color6"/>
                    </div>
                </div>
            </div>
            <div class="content-item" id="content13">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color13"/>
                    </div>
                    <div class="item">
                        교복 셔츠
                    </div>
                </div>
            </div>
            <div class="content-item" id="content14">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color14"/>
                    </div>
                    <div class="item">
                        교복 치마
                    </div>
                </div>
            </div>
            <div class="content-item" id="content15">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color15"/>
                    </div>
                </div>
            </div>
            <div class="content-item" id="content16">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color16"/>
                    </div>
                </div>
            </div>
            <div class="content-item" id="content17">
                <div class="item-grid">
                    <div class="item">
                        <input class="colorinput" type="color" v-model="color17"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="maker-wrapper">
        <div id="maker1" class="maker">
            <div id="titleinput">
                <div>FeatherMOE</div>
                <input v-model="characterName" />
            </div>
            <Svg src="/svg/skin-fill.svg" :fill=color0 :key=color0></Svg>
            <Svg src="/svg/face-fill.svg" :fill=color5 :key=color5></Svg>
            <Svg src="/svg/eyebrows-stroke.svg" :stroke=color1 :key=color1 class="stroke"></Svg>
            <Svg src="/svg/lefteyewhite-fill.svg" :fill=color2_1 :key=color2_1></Svg>
            <Svg src="/svg/righteyewhite-fill.svg" :fill=color2_1 :key=color2_1></Svg>
            <Svg src="/svg/lefteye-fill.svg" :fill=color2 :key=color2></Svg>
            <Svg src="/svg/righteye-fill.svg" :fill=color3 :key=color3></Svg>
            <Svg src="/svg/pupil-fill.svg" fill="#33009999"></Svg>
            <Svg src="/svg/highlight-fill.svg" fill="#ffffff"></Svg>
            <Svg src="/svg/lefteye-stroke.svg" stroke="#000"></Svg>
            <Svg src="/svg/righteye-stroke.svg" stroke="#000"></Svg>
            <Svg src="/svg/mouth-stroke.svg" :stroke=color4 :key=color4 class="stroke"></Svg>
            <Svg src="/svg/hair-fill.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/shirt-fill.svg" :fill=color13 :key=color13></Svg>
            <Svg src="/svg/shirt-stroke.svg" :stroke=color13 :key=color13 class="stroke"></Svg>
            <Svg src="/svg/skirt-fill.svg" :fill=color14 :key=color14></Svg>
            <Svg src="/svg/skirt-stroke.svg" :stroke=color14 :key=color14 class="stroke"></Svg>
            <Svg src="/svg/basic-cut.svg" stroke="#55339955"></Svg>
            <Svg src="/svg/basic-fold.svg" stroke="#00000011"></Svg>
        </div>
        <div id="maker2" class="maker">
            <Svg src="/svg/back-fill.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/bang-fill.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/rightside-fill.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/leftside-fill.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/rightside-stroke.svg" stroke="#55339955"></Svg>
            <Svg src="/svg/leftside-stroke.svg" stroke="#55339955"></Svg>
            <Svg src="/svg/bang-stroke.svg" :fill=color6 :key=color6></Svg>
            <Svg src="/svg/bang-highlight.svg" fill="#ffffdd99" ></Svg>
            <Svg src="/svg/bang-stroke.svg" stroke="#55339955"></Svg>
            <Svg src="/svg/back-stroke.svg" stroke="#55339955"></Svg>
            <Svg src="/svg/back-fold.svg" stroke="#00000011"></Svg>
        </div>
    </div>
</template>

<script setup>
    
    const characterName = ref('캐릭터 이름')
    const color0 = ref('#fff0eb')
    const color1 = ref('#86D7FF')
    const color2 = ref('#86D7FF')
    const color2_1 = ref('#ffffff')
    const color3 = ref('#86D7FF')
    const color4 = ref('#ff9ead')
    const color5 = ref('#ffc7cd')
    const color6 = ref('#86D7FF')
    const color13 = ref('#ffffff')
    const color14 = ref('#86D7FF')
    const color15 = ref('#86D7FF')
    const color16 = ref('#ffffff')
    const color17 = ref('#86D7FF')

    const tabclick = function(n) {
        document.querySelector('.tab-item.act').classList.remove('act')
        document.querySelector(`#tab${n}`).classList.add('act')
        document.querySelector('.content-item.act').classList.remove('act')
        document.querySelector(`#content${n}`).classList.add('act')
    }

</script>

<style lang="css">

    #tab-wrapper {
        margin: 0 auto;
        width: 100%;
        max-width: 1000px;
    }

    #tab-items {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        gap: 10px;
        overflow-x: auto;
    }

    .tab-item {
        min-width: 100px;
        height: 4rem;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: 'inadoong';
        background-color: white;
        border: 1px solid var(--line);
        font-size: 1.7rem;
        border-radius: 10px;
    }

    .tab-item.act {
        background-color: var(--accent);
        color: white;
        border: 0;
    }

    .content-item.act {
        border-radius: 10px;
        border: 1px solid var(--line);
        margin: 10px 0;
        display: block;
    }

    .content-item {
        display: none;
    }

    .item-grid {
        margin: 10px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr; 
        gap:10px;
    }

    .item {
        aspect-ratio: 1;
        border-radius: 5px;
        border: 1px solid var(--line);
        position: relative;
        overflow: hidden;
    }

    #maker-wrapper {
        width: 100%;
        height: 70vw;
        max-width: 1000px;
        max-height: 700px;
        margin: 0 auto;
        border: 1px solid var(--line);
        border-radius: 10px;
        background-color: var(--accentbg);
        display: flex;
    }

    #maker-wrapper .maker {
        position: relative;
        height: 70vw;
        max-height: 700px;
        width: 50vw;
        max-width: 500px;
    }

    #maker1 {
        border-right: 1px solid var(--accent);
    }

    #titleinput {
        position: absolute;
        top: min(1.5vw, 15px);
        left: min(2.5vw, 25px);
        z-index: 99;
    }

    #titleinput > div {
        font-size: min(1vw, 10px);
        margin-bottom: 0;
        padding-bottom: 0;
    }

    #titleinput > input {
        font-size: min(2.5vw, 25px);
        border: 0;
        height: min(3vw, 30px);
    }

    .colorinput {
        position: absolute;
        width: 110%;
        height: 110%;
        top: -5px;
        left: -5px;
    }

    .stroke {
        filter: saturate(200%) brightness(80%) contrast(85%);
    }
</style>