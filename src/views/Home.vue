<template>
    <my-page title="地理" :page="page">
        <app-list :data="groups" />
    </my-page>
</template>

<script>
    export default {
        data () {
            return {
                groups: [
                    {
                        // name: '分类',
                        apps: [
                            {
                                name: '地球',
                                desc: '',
                                icon: '/static/img/earth.svg',
                                to: 'xxx',
                                href: 'https://earth.yunser.com/',
                                target: '_blank'
                            },
                            {
                                name: '区号代码及时差',
                                desc: '国家区号代码及时差',
                                icon: '/static/img/earth.svg',
                                to: '/country'
                            },
                            {
                                name: '各国首都列表',
                                desc: '',
                                icon: '/static/img/earth.svg',
                                to: '/capital'
                            }
                        ]
                    }
                ],
                page: {
                    menu: [
                                                {
                            type: 'icon',
                            icon: 'search',
                            href: 'https://search.yunser.com?utm_source=geography',
                            target: '_blank',
                            title: '应用搜索'
                        },
                        {
                            type: 'icon',
                            icon: 'apps',
                            href: 'https://app.yunser.com?utm_source=geography',
                            target: '_blank',
                            title: '应用'
                        }
                    ]
                }
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>
