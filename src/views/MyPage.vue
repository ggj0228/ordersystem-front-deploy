<template>
    
    <!-- 내 정보 조회 -->
    <!-- 문자열로 props를 넘길경우 변수명="값", 그외에는 :변수명 형태로 전달 -->
    <MemberDetailComponent
    :isMyPage="true" pageTitle="내회원정보"
    />

    <!-- 내 주문내역 조회 -->
    <OrderListComponet
    :isMyPage="true"
    />
</template>
<script>
import MemberDetailComponent from '@/components/MemberDetailComponent.vue';
import OrderListComponet from '@/components/OrderListComponet.vue';

export default{
    components:{
        MemberDetailComponent, OrderListComponet
    }
}
</script>