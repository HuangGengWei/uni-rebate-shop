<template>
	<view class="content">
	<section class="aui-flexView">
	    <section class="aui-scrollView">
			<QStabs :tabs="tabs" :current="current" width="180" @change="change($event)"></QStabs>
	        <div class="aui-tab" data-ydui-tab>
	            <!-- <ul class="tab-nav">
	                <li class="tab-nav-item tab-active">
	                    <a href="javascript:;">精选</a>
	                </li>
	                <li class="tab-nav-item">
	                    <a href="javascript:;">潮科技</a>
	                </li>
	                <li class="tab-nav-item">
	                    <a href="javascript:;">生活家</a>
	                </li>
	                <li class="tab-nav-item">
	                    <a href="javascript:;">时尚馆</a>
	                </li>
	            </ul> -->
	            <div class="tab-panel">
	                <div class="tab-panel-item" :class="[current===0?'tab-active':'']">
	                    <div class="tab-item">
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-001.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                          <i>￥6499</i>        
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-002.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥6499</i>   
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-003.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥6499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-004.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥6499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-005.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥6499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-006.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥6499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                    </div>
	                </div>
	                <div class="tab-panel-item" :class="[current===1?'tab-active':'']">
	                    <div class="tab-item">
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-007.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>智能手表男续航30天 成人wifi计步器GPS运动心率支付创新双层屏 安卓苹果</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥1499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-008.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple Watch Series 3智能手表（GPS款 42毫米 深空灰色铝金属表壳 黑色运动型表带 MTF32CH/A）</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                            <i>￥2499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-009.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>智力快车 R3金小帅才子儿童智能机器人3.0第三代触屏学习机3-6-12岁教育陪伴早教语音对话人工玩具小胖</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥6499</i>
	                                        </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-004.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-005.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-006.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                    </div>
	                </div>
	                <div class="tab-panel-item" :class="[current===2?'tab-active':'']">
	                    <div class="tab-item">
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-001.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-002.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-003.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-004.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-005.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-006.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                    </div>
	                </div>
	                <div class="tab-panel-item" :class="[current===3?'tab-active':'']">
	                    <div class="tab-item">
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-001.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-002.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-003.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-004.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-005.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                        <a href="javascript:;" class="aui-flex b-line">
	                            <div class="aui-product-img">
	                                <img src="/static/picture/iphone-img-006.png" alt="">
	                                <span class="aui-product-make">预约</span>
	                            </div>
	                            <div class="aui-flex-box">
	                                <p>Apple iPhone XR (A2108) 64GB 白色 移动联通电信4G手机 双卡双待</p>
	                                <div class="aui-flex aui-flex-clear">
	                                    <div class="aui-flex-box">
	                                        <span>预约价</span>
	                                        <span class="aui-product-price">
	                                                    <i>￥</i>
	                                                    6499
	                                                </span>
	                                    </div>
	                                    <div class="aui-product-button">
	                                        <span>27833人预约</span>
	                                        <button>立即预约</button>
	                                    </div>
	                                </div>
	                            </div>
	                        </a>
	                    </div>
	                </div>
	            </div>
	        </div>
	    </section>
	</section>	
	</view>
</template>
<script>
	import '@/static/css/style.css';
	import QStabs from '@/components/QS-tabs/QS-tabs.vue';
	export default {
		data() {
			return {
				current: 0,
				tabs: ['精选', '潮科技', '生活家', '时尚馆'],
			}
		},
		components:{
			QStabs
		},
		onLoad() {
		},
		methods: {
			change(index) {
				//console.log('index',index);
				this['current'] = index;
			}
		}
	}
</script>
