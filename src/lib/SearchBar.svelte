<script>

</script>

<form>
    <div class="search my-4 my-xl-5 mx-auto d-flex justify-content-center">
        <input class="p-3 rounded-start-4" type="text" name="search" placeholder="Search for any IP address or domain">
        <button class="p-3 px-xl-4 rounded-end-4">
            <img src="../icon-arrow.svg" alt="">
        </button>
    </div>
</form>

<style>
input {
  cursor: pointer;
  width: 40rem;
  border: none;
  font-size: clamp(1em, 3vw, 1.4em);

  &:focus {
    outline: none;
  }
}

button {
  border: none;
  background-color: black;
  position: relative;
  overflow: hidden;

  &:hover::after {
    content: '';
    position: absolute;
    inset: 0;
    background-color: rgba(255, 255, 255, 0.132);
  }
}

@media (max-width : 576px) {}

@media (min-width : 577px) {}

@media (min-width : 1201px) {}
</style>
