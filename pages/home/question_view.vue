<template>
	<!-- 问题详情页 -->
	<view class="page_home" id="home_question_view">
		<!-- 页头 -->
		<mm_header>
			<!-- 外套 -->
			<mm_warp></mm_warp>
		</mm_header>
		<!-- 页主体 -->
		<mm_bodyer>
			<!-- 外套 -->
			<mm_warp>
				<!-- 栅格 -->
				<mm_grid col="1" class="space_big">
					<!-- 格子 -->
					<mm_col>
						<!-- 问题详情 -->
						<mm_block>
							<mm_head>
								<mm_title>{{ obj.title }}</mm_title>
							</mm_head>
							<mm_body class="pa" v-html="obj.content">
							</mm_body>
							<mm_foot>
								<!-- 上下篇问题 -->
							</mm_foot>
						</mm_block>
					</mm_col>
				</mm_grid>
			</mm_warp>
		</mm_bodyer>
	</view>
</template>

<script>
	import mixin from '@/mixins/page'

	export default {
		mixins: [mixin],
		components: {},
		data() {
			return {
				oauth: true,
				url_get_obj: "~/paper/id",
				query: {
					id: "",
					title: ""
				},
				obj: {
					author: "",
					content: "",
					description: "",
					display: 0,
					grouping: "",
					id: 0,
					keyWords: [],
					state: 0,
					time: "2019-06-14 15:01:16",
					title: "",
					users: []
				}
			}
		}
	}
</script>

<style>
</style>
