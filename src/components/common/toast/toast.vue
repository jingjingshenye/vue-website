<template>
</template>

<script>
  export default {
  }
</script>

<style scoped>
	.vue-toast{
		position:fixed;
		background:rgba(0,0,0,0.3);
		font-size:14px;
		color:#fff;
		line-height:1.5;
		padding: 3px 10px;
		width:auto;
		border-radius:6px;
		max-width:300px;
		display:inline-block;
		user-select: none;
		word-wrap: break-word;
		opacity:1;
		z-index: 10000000;
		cursor:default;
		&.bottom{
			bottom: 10%;
			left:50%;
			transform:translate(-50%,0);
			&.fade-up-enter{
				opacity: 0;
				transform:translate(-50%,10px);
			}
		}
		&.center{
			top: 50%;
			left:50%;
			transform:translate(-50%,-50%);
			&.fade-up-enter{
				opacity: 0;
				transform:translate(-50%,calc(-50% + 10px));
			}
		}
		&.top{
			top: 10%;
			left:50%;
			transform:translate(-50%,0);
			&.fade-up-enter{
				opacity: 0;
				transform:translate(-50%,10px);
			}
		}
		&.fade-up-enter-to,&.fade-up-leave-to{
			transition: all .3s ease;
		}
		&.fade-up-leave-to{
			opacity: 0;
		}
			
	}
</style>