<template>
	<!-- DBD流水页面 -->
	<mm_page class="page_user" id="user_bill_btc">
		<mm_bodyer>
			<mm_warp>
				<mm_grid>
					<mm_col>
						<mm_block>
							<mm_head>
								<mm_title>2019年5月</mm_title>
							</mm_head>
							<mm_body class="lr">
								<mm_list col="1">
									<mm_item class="big">
										<mm_main>
											<mm_title>挖矿产出</mm_title>
											<mm_desc>
												5月20日 10:50
											</mm_desc>
											<mm_desc class="font_success">
												<text>+0.013</text>
											</mm_desc>
										</mm_main>
									</mm_item>
									<mm_item class="big">
										<mm_main>
											<mm_title>购买DBD</mm_title>
											<mm_desc>
												5月20日 10:50
											</mm_desc>
											<mm_desc class="font_warning">
												<text>-0.08323</text>
											</mm_desc>
										</mm_main>
									</mm_item>
								</mm_list>
							</mm_body>
						</mm_block>
					</mm_col>
					<mm_col>
						<mm_block>
							<mm_head>
								<mm_title>2019年4月</mm_title>
							</mm_head>
							<mm_body class="lr">
							<mm_list col="1">
								<mm_item class="big">
									<mm_main>
										<mm_title>回购DBD</mm_title>
										<mm_desc>
											5月20日 10:50
										</mm_desc>
										<mm_desc class="font_success">
											<text>+0.01332</text>
										</mm_desc>
									</mm_main>
								</mm_item>
								<mm_item class="big">
									<mm_main>
										<mm_title>申请提币</mm_title>
										<mm_desc>
											5月20日 10:50
										</mm_desc>
										<mm_desc class="font_warning">
											<text>-0.08</text><text class="unit">btc</text>
										</mm_desc>
									</mm_main>
								</mm_item>
							</mm_list>
							</mm_body>
						</mm_block>
					</mm_col>
				</mm_grid>
			</mm_warp>
		</mm_bodyer>
	</mm_page>
</template>

<script>
	import mixin from '@/mixins/page'
	export default {
		mixins: [mixin],
		data() {
			return {
				oauth: true
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.font_success, .font_warning {
		position: absolute;
		right: 1rem;
		top: 50%;
		transform: translate(0, -50%);
		font-size: 0.875rem;
		font-weight: 600;
	}
</style>
