<template>
<div class="contact mt-4">
    <div class="container">
        <div class="row">
            <div class="col-12 col-lg-6 my-4">
                <h1 class="text-light text-center mb-3">Contact Us</h1>
                <div class="row">
                    <div class="col-12 col-md-6">
                        <div class="form-floating mb-3">
                            <input type="email" class="form-control" id="floatingInput" placeholder="name">
                            <label for="floatingInput">Name</label>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <div class="form-floating mb-3">
                            <input type="text" class="form-control" id="floatingInput2" placeholder="name@example.com">
                            <label for="floatingInput2">Email</label>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-12">
                        <div class="form-floating mb-3">
                            <textarea class="form-control" placeholder="Leave your massage here" id="floatingTextarea2" style="height: 100px"></textarea>
                            <label for="floatingTextarea2">Massage</label>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="d-grid">
                        <button type="button" class="btn btn-outline">Send Massage</button>
                    </div>
                </div>
            </div>
            <div class="col-12 col-lg-6 text-center text-light mb-4 my-lg-auto">
                <img src="../assets/img/logo.png" alt="" class="mb-4" />
                <h6>Main Branch Adrress : 228 Park Ave S, New York, United State</h6>
                <h6>Phone : (99)999-9999</h6>
                <h6>Mobile : 9999-9999-9999</h6>
                <h6>Email : coffecup@dummy.com</h6>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
.contact{
    background-color: #122341;
}

h1{
    font-family: 'Cormorant Garamond', serif;
    font-size: 3rem;
}

.btn-outline {
  --bs-btn-font-weight: 600;
  --bs-btn-color: var(--bs-white);
  --bs-btn-bg: transparent;
  --bs-btn-border-color: var(--bs-white);
  --bs-btn-border-radius: .5rem;
  --bs-btn-hover-color: var(--bs-black);
  --bs-btn-hover-bg: var(--bs-white);
  --bs-btn-hover-border-color: transparent;
  --bs-btn-focus-shadow-rgb: var(--bd-violet-rgb);
  --bs-btn-active-color: var(--bs-btn-color);
  --bs-btn-active-bg: #{shade-color($bd-violet, 20%)};
  --bs-btn-active-border-color: var(--bs-btn-border-color);
}
</style>