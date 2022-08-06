<script>
    export let text = "Studio Ghibli, dirigida y creada por Hayao Miyazaki en 1988. Tras realizar esta película, se adoptó como logotipo del estudio a los Totoros. Es la tercera película del estudio tras su fundación.";
    export let image = "https://i.pinimg.com/564x/13/ce/1a/13ce1a83c6728beb5dfcb4f3149f5bd0.jpg";
</script>

<style>
    /* FLIP CARD */
.flip-card {
  flex: 1 0 auto;
  margin: 0 50px;
  width: 320px;
  height: 504px;
  perspective: 2000px;

  font-size: xx-small;
}
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
  border-radius: 28px;
  transition: all 550ms cubic-bezier(0.1, 0.22, 0.8, 1.13);
  transform-style: preserve-3d;
}
.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 28px;
  backface-visibility: hidden;
}
.flip-card-front {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.flip-card-back {
  font-size: 1.25rem;
  text-align: center;
  display: grid;
  place-items: center;
  padding: 32px;
  background-color: #B1CFC8;
  transform: rotateY(180deg);
}
.flip-card:hover .flip-card-inner {
  transform: rotateY(-180deg);
}
</style>

<div class="flip-card">
    <div class="flip-card-inner">
        <div class="flip-card-front" style="background-image: url({image});">

        </div>
        <div class="flip-card-back">
        {text}
        </div>
    </div>
</div>

