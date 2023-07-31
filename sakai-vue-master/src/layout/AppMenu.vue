<script setup>
import { ref } from 'vue';

import AppMenuItem from './AppMenuItem.vue';

const model = ref([
    {
        label: 'Ana Sayfa',
        items: [{ label: 'Gösterge Paneli', icon: 'pi pi-fw pi-home', to: '/' }]
    },
    {
        label: 'Kullanıcı Arayüzü',
        items: [

            { label: 'Üyeler', icon: 'pi pi-id-card', to: '/uikit/table' },
            { label: 'Komisyon Hesaplama', icon: 'pi pi-calculator', to: '/uikit/tree' },
            { label: 'Tamamlanmış Ödemeler', icon: 'pi pi-tablet', to: '/uikit/panel' },
            { label: 'Menu', icon: 'pi pi-fw pi-bars', to: '/uikit/menu', preventExact: true },
            { label: 'Kayıtlı Kartlar', icon: 'pi pi-credit-card', to: '/uikit/file' }           
        ]
    },
    {
        label: 'Haber Sayfaları',
        items: [
            
            { label: 'Duyurular', icon: 'pi pi-bell', to: '/utilities/icons' },
            { label: 'Sayfalar', icon: 'pi pi-globe', to: '/uikit/formlayout' }
        ]
    },
    {
        label: 'Pazar Yeri',
        items: [
        {
                label: 'Mağaza Bilgileri',
                icon: 'pi pi-cart-plus',
                items: [
                { 
                    label: 'Mağazalarım',
                    icon: 'pi pi-cart-plus',
                    to: '/uikit/media' 
                },
                { 
                    label: 'Mağaza Notlarım',
                    icon: 'pi pi-cart-plus',
                    to: '/blocks', badge: 'NEW' 
                },
                {
                     label: 'Mağazalar',
                     icon: 'pi pi-cart-plus', 
                     to: '/uikit/charts' 
                },
                {
                     label: 'Mağaza Raporu',
                     icon: 'pi pi-cart-plus', 
                     to: '/uikit/charts' 
                }
                
                ]
            },
            {
                label: 'Ürün Bilgileri',
                icon: 'pi pi-shopping-bag',
                items: [
                { 
                    label: 'Ürünlerim',
                    icon: 'pi pi-fw pi-list',
                    to: '/uikit/list'
                },
                { 
                    label: 'Ürün Kategorisi',
                    icon: 'pi pi-database', 
                    to: '/uikit/floatlabel' 
                },
                
                ]
            },
        ]
    },
    {
        label: 'Yönetim',
        icon: 'pi pi-fw pi-briefcase',
        to: '/pages',
        items: [
        {
                
                label: 'Geri Bildirim',
                icon: 'pi pi-comments',
                items: [
                { 
                    label: 'Şikayet',
                    icon: 'pi pi-fw pi-check-square',
                    to: '/uikit/input'
                },
                { 
                    label: 'Sorgulamak',
                    icon: 'pi pi-question-circle', 
                    to: '/uikit/floatlabel' 
                },
                ]
            },
            {
                
                label: 'Mesaj İşlemleri',
                icon: 'pi pi-comment',
                items: [
                { 
                    label: 'E-mail ve Mesaj Gönder',
                    icon: 'pi pi-envelope',
                    to: '/uikit/message' 
                },
                { 
                    label: 'E-mail Plan',
                    icon: 'pi pi-calendar',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'E-mail Şablonları',
                    icon: 'pi pi-file',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'E-mail Logları',
                    icon: 'pi pi-book',
                    to: '/uikit/invalidstate' 
                },
                ]
            },
            
            {
                
                label: 'Ayarlar',
                icon: 'pi pi-cog',
                items: [
                { 
                    label: 'Loglar',
                    icon: 'pi pi-bookmark-fill',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Sözleşme',
                    icon: 'pi pi-pencil',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Modüller',
                    icon: 'pi pi-briefcase',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Güncellemeler',
                    icon: 'pi pi-cloud-upload',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Dil secimi',
                    icon: 'pi pi-language',
                    to: '/uikit/invalidstate' 
                },
                ]
            },
            {
                
                label: 'Görünüm',
                icon: 'pi pi-desktop',
                items: [
                { 
                    label: 'Şablonlar',
                    icon: 'pi pi-clone',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Temalar',
                    icon: 'pi pi-inbox',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Ayar',
                    icon: 'pi pi-wrench',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Edition',
                    icon: 'pi pi-user-edit',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Banner',
                    icon: 'pi pi-images',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'Video',
                    icon: 'pi pi-video',
                    to: '/uikit/invalidstate' 
                },
                ]
            },
            {
                label: 'Banka ve Komisyon',
                icon: 'pi pi-wallet',
                items: [
                { 
                    label: 'Banka Ayarları',
                    icon: 'pi pi-id-card',
                    to: '/uikit/input'
                },
                { 
                    label: 'Banka Komisyon',
                    icon: 'pi pi-fw pi-bookmark', 
                    to: '/uikit/floatlabel' 
                },
                {
                    label: 'Banka Havale /EFT',
                    icon: 'pi pi-credit-card',
                    to: '/uikit/invalidstate' 
                },
                ]
            },
            {
                label: 'Ödemeler',
                icon: 'pi pi-shopping-cart',
                items: [
                { 
                    label: 'Bakiyeler',
                    icon: 'pi pi-fw pi-check-square',
                    to: '/uikit/input'
                },
                { 
                    label: 'Başarılı Ödemeler',
                    icon: 'pi pi-fw pi-bookmark', 
                    to: '/uikit/floatlabel' 
                },
                { 
                    label: 'Başarısız Ödemeler',
                    icon: 'pi pi-fw pi-exclamation-circle',
                    to: '/uikit/invalidstate' 
                },
                { 
                    label: 'İadeler',
                    icon: 'pi pi-fw pi-mobile',
                    to: '/uikit/button',
                    class: 'rotated-icon'
                },
                ]
            },
            {
                label: 'Admin',
                icon: 'pi pi-user-plus',
                items: [
                { 
                    label: 'Yöneticiler',
                    icon: 'pi pi-user-edit',
                    to: '/auth/login'
                },
                { 
                    label: 'Üyeler',
                    icon: 'pi pi-user', 
                    to: '/uikit/floatlabel' 
                },
                { 
                    label: 'Kullanıcılar',
                    icon: 'pi pi-users',
                    to: '/uikit/invalidstate' 
                }, 
                ]
            },
            {
                label: 'Dosyalar',
                icon: 'pi pi-file-edit',
                items: [
                { 
                    label: 'Video',
                    icon: 'pi pi-play',
                    to: '/uikit/input'
                },
                { 
                    label: 'Fotoğraf',
                    icon: 'pi pi-image', 
                    to: '/uikit/floatlabel' 
                }, 
                ]
            },
            {
                label: 'Üyeler ekle',
                icon: 'pi pi-fw pi-pencil',
                to: '/pages/crud'
            },
            {
                label: 'Timeline',
                icon: 'pi pi-fw pi-calendar',
                to: '/pages/timeline'
            },
            {
                label: 'Not Found',
                icon: 'pi pi-fw pi-exclamation-circle',
                to: '/pages/notfound'
            },
            {
                label: 'Empty',
                icon: 'pi pi-fw pi-circle-off',
                to: '/pages/empty'
            }
        ]
    },
    
   
]);
</script>

<template>
    <ul class="layout-menu">
        <template v-for="(item, i) in model" :key="item">
            <app-menu-item v-if="!item.separator" :item="item" :index="i"></app-menu-item>
            <li v-if="item.separator" class="menu-separator"></li>
        </template>
    </ul>
</template>

<style lang="scss" scoped></style>
