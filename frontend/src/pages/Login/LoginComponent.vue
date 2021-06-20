<template>
  <div class="main">
    <div class="login">
      <div class="content-login">
        <header>
          <h1>Login do sistema</h1>
        </header>
        <div class="form">
          <form >
            <div class="form-group">
              <label for="exampleInputEmail1" class="mt-2">E-mail</label>
              <input
                type="email"
                class="form-control mt-2"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
                placeholder="Informe o e-mail"
              />
            </div>
            <div class="form-group">
              <label for="exampleInputPassword1" class="mt-2">Senha</label>
              <input
                type="password"
                class="form-control mt-2"
                id="exampleInputPassword1"
                placeholder="Informe a senha"
              />
            </div>
            <button type="submit" class="btn btn-primary mt-3" @click.prevent="login">Entrar</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "LoginComponent",
    data(){
        return{}
    },
    methods: {
        login(){
            this.$router.push({name: 'home'})
        }
    }
};
</script>

<style lang="scss" src="./style.scss" scoped />
