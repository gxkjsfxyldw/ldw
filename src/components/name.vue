
<style>
	
        *{
            padding: 0;
            margin: 0;
			text-decoration:none;
        }
        form input{
            width:450px;
            height: 40px;
            padding-left: 10px;
            border-radius: 5px;
            float: right;
        }
        ul{
            margin: 0;
            padding: 0;
			
        }
        .ul1 li{
           
            list-style-type: none;
            display: inline;
            float: left;
            padding: 10px 32px;

        }
		.ul1 li a{ 
			text-decoration:none;
		}
        .ul1 li:hover{
            background-color: #fff;
        }
        .ul2 li{
            list-style-type: none;
            padding: 5px;
        }

        p{
            margin-left: 30px;
            display: inline;
            background-color: #55ff00;
            padding: 7px 20px;
        }
        p:hover{
            background-color: #ffff00;
        }
</style>
<style type="text/css" scoped="scoped">
	@import url("https://cdn.staticfile.org/twitter-bootstrap/5.1.1/css/bootstrap.min.css");
</style>


<template>
	
 <div class="container-fluid" style="background-color: #F6F6F6;">
        <div class="row" >
            <div class="col-5" style="height: 100px;text-align: center;">
                <br><h1 style="font-family: 'Stencil';">{{RUNOOB}}<span style="color: #3f8ab9;">{{com}}</span></h1>
            </div>
            <div class="col-6" >
                <form action="">
                    <br>
                    <input type="text" placeholder="搜索...">
                </form>
            </div>
        </div>
        <div class="row" style="background-color: #3285b9;">
            <div class="col-9" style="margin: 0 auto;">
                <ul class="ul1" >
                    <li v-for="item in items">
						<a href="#"style="color: #57bfff;">{{item}}</a>
					</li>
                </ul>
            </div>
        </div>
<br>
        <div class="row" style="height: 540px;color: #54a3b9;">
            <div class="col-1" style="text-align: center;margin-left: 170px;">
                <ul class="ul2">
                    <li v-for="item1 in items">
                        {{item1}}
                    </li>
                </ul>
            </div>
            <div class="col-7" style="margin-left: 30px;">
                <h2 style="font-family: '华文中宋';"><span style="color: #54a3b9;">{{uid}}</span>{{ldw}}</h2>
                <iframe src="https://www.runoob.com/" width="100%" height="450px" ></iframe>
            </div>
            <div class="col-2" style="color: #54a3b9;">>
                <ul class="ul2">
                    <li v-for="item1 in items1">
                        {{item1}} 
                    </li>
                </ul>
            </div>
        </div>
    
    </div>
</template>

<script>
	export default {
		ldw: 'HelloLdw',
		props: {
			msg: String
		},
		methods: {


		},
		data() {
			return {

				title: 'LDW.COM',
				items: [
					'LDW',
					'LDW',
					'LDW',
					'LDW',
					'LDW',
					'LDW',
					'LDW',
					
				],
				leftTitle: 'LDW 教程',
				items1: [
					'LDW 教程',
					'LDW 简介',
					'LDW',
					'LDW 元素',
					'LDW 属性',
					'LDW 标题',
					'LDW 段落',
					'LDW 文本格式',
					'LDW 链接',
					'LDW 头部',
				],
				uid: '',
				name: '',
				RUNOOB:'LDW',
				com:'.com',
				




			}
		}
	}
</script>

