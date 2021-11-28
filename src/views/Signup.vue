<template>
  <div class="about">
    <h1>This is an signup page</h1>
    <div class="container">
      <div class="row">
        <div class="col-sm"></div>
        <div class="col-sm">
          <form>
            <div class="form-group">
              <label for="ime">Name:</label>
              <input
                type="text"
                id="ime"
                placeholder="Enter your name..."
                class="form-control"
              />
            </div>

            <div class="form-group">
              <label for="prezime">Surname:</label>
              <input
                type="text"
                id="prezime"
                placeholder="Enter your surname..."
                class="form-control"
              />
            </div>

            <div class="form-group">
              <label for="username">Username:</label>
              <input
                type="text"
                id="username"
                placeholder="Enter your username..."
                class="form-control"
              />
            </div>

            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input
                type="email"
                class="form-control"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
                placeholder="Enter email"
              />
              <small id="emailHelp" class="form-text text-muted"
                >We'll never share your email with anyone else.</small
              >
            </div>

            <div class="form-group">
              <label for="exampleInputPassword1">Password</label>
              <input
                type="password"
                class="form-control"
                id="exampleInputPassword1"
                placeholder="Password"
              />
            </div>

            <div class="form-group">
              <label for="confirm">Confirm password</label>
              <input
                type="password"
                class="form-control"
                id="confirm"
                placeholder="Confirm password"
              />
            </div>

            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>
        <div class="col-sm"></div>
      </div>
    </div>
  </div>
</template>
