<template>
	<view class="homepage">
		<view class="people">
			<view class="headImg">
				<image src="@/static/peo3.png"></image>
			</view>
			<view class="info">
				<view class="nick">
					<text>新手982413</text>
					<view class="sex">
						<!-- uview-plus ui库的 -->
						<!-- <u-icon name="man" color="#ffffff" size="24"></u-icon> -->
					</view>
				</view>
				<view class="grade">
					<view>
						<image src="@/static/shield.png"></image>
						<text>0</text>
					</view>
					<view>
						<image src="@/static/vip.png"></image>
						<text>0</text>
					</view>
				</view>
				<view class="userId">
					<image src="@/static/id.png"></image>
					<view class="number">
						<text>982413</text>
						<text>复制</text>
					</view>
				</view>
			</view>
			<view class="space">
				<text>空间</text>
				<!-- uview-plus ui库的 -->
				<!-- <u-icon name="arrow-right" color="#000000" size="20"></u-icon> -->
			</view>
		</view>
		<view class="list">
			<view class="item">
				<view class="text">
					<text>0</text>
					<text>关注</text>
				</view>
				<!-- uview-plus ui库的 -->
				<!-- <u-line direction="col" color="#979797 " length="32rpx"></u-line> -->
			</view>
			<view class="item">
				<view class="text">
					<text>0</text>
					<text>粉丝</text>
				</view>
				<!-- uview-plus ui库的 -->
				<!-- <u-line direction="col" color="#979797 " length="32rpx"></u-line> -->
			</view>
			<view class="item">
				<view class="text">
					<text>0</text>
					<text>动态</text>
				</view>
				<!-- uview-plus ui库的 -->
				<!-- <u-line direction="col" color="#979797 " length="32rpx"></u-line> -->
			</view>
			<view class="item">
				<view class="text">
					<text>0</text>
					<text>访客</text>
				</view>
			</view>
		</view>
		<view class="infos">
			<view class="open-vip">
				<image src="@/static/vip01.png"></image>
				<text class="text">未开通 至尊爵位，尊享体验！</text>
				<text class="button">开通爵位</text>
			</view>
			<view class="tool">
				<view>
					<image src="@/static/member.png"></image>
					<text>我的公会</text>
				</view>
				<view>
					<image src="@/static/shop.png"></image>
					<text>道具商城</text>
				</view>
				<view>
					<image src="@/static/house.png"></image>
					<text>我的房间</text>
				</view>
				<view>
					<image src="@/static/money.png"></image>
					<text>我的钱包</text>
				</view>
			</view>
			<view class="set">
				<view>
					<image class="icon" src="@/static/pic03.png"></image>
					<text>最近进房</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
				<view>
					<image class="icon" src="@/static/pic02.png"></image>
					<text>优惠券</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
				<view>
					<image class="icon" src="@/static/pic05.png"></image>
					<text>我的等级</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
				<view>
					<image class="icon" src="@/static/pic04.png"></image>
					<text>我的守护</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
				<view>
					<image class="icon" src="@/static/pic06.png"></image>
					<text>赏金任务-好友召回</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
			</view>
			<view class="service">
				<view>
					<image class="icon" src="@/static/pic02.png"></image>
					<text>兑换奖励</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
				<view>
					<image class="icon" src="@/static/pic07.png"></image>
					<text>在线客服</text>
					<image class="right" src="@/static/Clipped.png"></image>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value: 1,
				value1: 0
			}
		}
	}
</script>

<style lang="scss" scoped>
	.homepage {
		width: 100%;
		height: 1624rpx;
		background: linear-gradient(1deg, rgba(247, 240, 255, 0.19) 0%, rgba(229, 232, 255, 0.2) 68%, rgba(231, 228, 255, 0.66) 100%);

		& text {
			color: #333333;
			font-family: PingFangSC-Semibold, PingFang SC;
		}

		// .bar {
		// 	.right {
		// 		display: flex;

		// 		& view {
		// 			width: 52rpx;
		// 			height: 52rpx;
		// 			margin-left: 26rpx;
		// 			border-radius: 26rpx;
		// 			background: #f0eeff;
		// 			display: flex;
		// 			justify-content: center;
		// 			align-items: center;
		// 			box-shadow: 0rpx -2rpx 2rpx 4rpx rgba(255, 255, 255, 0.5), 0rpx 4rpx 4rpx 0rpx rgba(197, 183, 211, 0.5), inset 0rpx 2rpx 6rpx 0rpx rgba(255, 255, 255, 0.5);

		// 			> image {
		// 				width: 32rpx;
		// 				height: 32rpx;
		// 			}
		// 		}
		// 	}
		// }

		.people {
			padding: 0 42rpx 28rpx 32rpx;
			display: flex;
			align-items: center;

			.headImg {
				> image {
					width: 166rpx;
					height: 166rpx;
					border-radius: 83rpx;
				}
			}

			.info {
				flex: 1;

				.nick {
					display: flex;

					> text {
						font-size: 36rpx;
						font-weight: 600;
						line-height: 50rpx;
					}

					.sex {
						width: 24rpx;
						height: 24rpx;
						border-radius: 12rpx;
						background: #61c9fd;
					}
				}

				.grade {
					display: flex;
					align-items: center;

					> view {
						display: flex;
						align-items: center;
						margin-right: 12rpx;

						& text {
							font-size: 20rpx;
							font-weight: 600;
							color: #ffffff;
							line-height: 28rpx;
							text-shadow: 0rpx 2rpx 4rpx rgba(0, 0, 0, 0.5);
						}

						& image {
							width: 28rpx;
							height: 30rpx;
						}

						&:last-child {
							> image {
								width: 40rpx;
								height: 40rpx;
							}

							> text {
								margin-left: -6rpx;
							}
						}
					}
				}

				.userId {
					width: 220rpx;
					display: flex;
					background: #f5f5ff;
					border-radius: 8rpx;
					box-shadow: 0rpx 2rpx 6rpx 0rpx rgba(0, 0, 0, 0.14), 0rpx -4rpx 6rpx 0rpx #ffffff;

					> image {
						width: 36rpx;
						height: 40rpx;
					}

					.number {
						flex: 1;
						display: flex;
						justify-content: center;

						> text {
							font-size: 24rpx;
							font-weight: 600;
							line-height: 40rpx;

							&:last-child {
								font-weight: 500;
								font-size: 22rpx;
								margin-left: 8rpx;
							}
						}
					}
				}
			}

			.space {
				display: flex;
				align-items: center;

				> text {
					font-size: 28rpx;
					line-height: 40rpx;
				}
			}
		}

		.list {
			width: 100%;
			display: flex;
			padding: 0 44rpx;
			box-sizing: border-box;

			.item {
				width: 25%;
				display: flex;
				justify-content: space-evenly;
				align-items: center;

				.text {
					display: flex;
					flex-direction: column;
					align-items: center;

					> text:first-child {
						font-size: 36rpx;
						font-family: CloudHeiChaoGBK;
						line-height: 48rpx;
						font-weight: 600;
					}

					> text:last-child {
						font-size: 24rpx;
						color: #999999;
						line-height: 34rpx;
					}
				}
			}
		}

		.infos {
			padding: 0 40rpx;

			.open-vip {
				width: 100%;
				height: 72rpx;
				background: linear-gradient(180deg, #f7e5b4 0%, #ffe6af 2%, #ebc075 100%);
				border-radius: 49rpx;
				display: flex;
				align-items: center;
				margin-top: 36rpx;
				padding: 0 24rpx 0 34rpx;
				box-sizing: border-box;

				> image {
					width: 48rpx;
					height: 48rpx;
				}

				.text {
					flex: 1;
					font-size: 24rpx;
					line-height: 34rpx;
					margin-left: 14rpx;
				}

				.button {
					width: 128rpx;
					height: 42rpx;
					background: linear-gradient(90deg, #4d4d4d 0%, #151515 100%);
					border-radius: 22rpx;
					font-size: 22rpx;
					color: #ffdfa9;
					line-height: 42rpx;
					text-align: center;
				}
			}

			.tool {
				display: flex;
				width: 100%;
				height: 172rpx;
				background: #ffffff;
				box-shadow: 0rpx 2rpx 22rpx 0rpx rgba(114, 118, 206, 0.27);
				border-radius: 28rpx;
				justify-content: space-evenly;
				margin: 22rpx 0;

				> view {
					display: flex;
					flex-direction: column;

					& text {
						font-size: 22rpx;
						font-weight: 600;
						color: #666666;
						line-height: 32rpx;
						text-shadow: 0rpx 4rpx 14rpx rgba(222, 148, 247, 0.6);
					}

					& image {
						width: 98rpx;
						height: 96rpx;
						margin-top: 10rpx;
					}
				}
			}

			.set {
				width: 100%;
				padding: 34rpx 24rpx 44rpx 34rpx;
				background: #ffffff;
				box-shadow: 0rpx 2rpx 28rpx 0rpx rgba(142, 146, 230, 0.27);
				border-radius: 28rpx;
				display: flex;
				flex-direction: column;
				justify-content: space-between;
				box-sizing: border-box;

				> view {
					display: flex;
					align-items: center;
					margin-bottom: 40rpx;

					& text {
						flex: 1;
						font-size: 28rpx;
						line-height: 40rpx;
						margin-left: 30rpx;
					}

					.icon {
						width: 36rpx;
						height: 36rpx;
					}

					.right {
						width: 40rpx;
						height: 40rpx;
					}
				}
			}

			.service {
				background: #ffffff;
				box-shadow: 0rpx 2rpx 28rpx 0rpx rgba(142, 146, 230, 0.27);
				border-radius: 28rpx;
				margin-top: 26rpx;
				padding: 34rpx 24rpx 44rpx 34rpx;
				display: flex;
				flex-direction: column;
				justify-content: space-between;

				> view {
					display: flex;
					align-items: center;
					margin-bottom: 40rpx;

					& text {
						flex: 1;
						font-size: 28rpx;
						line-height: 40rpx;
						margin-left: 30rpx;
					}

					.icon {
						width: 36rpx;
						height: 36rpx;
					}

					.right {
						width: 40rpx;
						height: 40rpx;
					}
				}
			}
		}
	}
</style>
