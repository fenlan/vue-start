<template>
<div class="layout">
    <Layout>
        <Header>Header</Header>
        <Layout>
          <Sider hide-trigger>Sider</Sider>
          <Content>Content</Content>
        </Layout>
        <Footer></Footer>
    </Layout>
</div>
</template>
<script>
import Header from './Header'
import Sider from './Sider'
import Content from './Content'

export default {
  components: {
    'Header': Header,
    'Sider': Sider,
    'Content': Content
  }
}
</script>

<style scope>
</style>
