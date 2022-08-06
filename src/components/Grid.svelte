<script>
	import { text } from 'svelte/internal';
    import Card from "./Card.svelte";
    let positions = [
        {
            text: "Enseñar al que no sabe",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/2-Ense%C3%B1ar-al-que-no-sabe.png",
        },
        {
            text: "corregir al que se equivoca",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/4-Corregir-al-que-esta-en-error.png",
        },
        {
            text: "Dar buen consejo al que lo necesita",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/1-Dar-buen-consejo-al-que-lo-necesita.png",
        },
        {
            text: "Perdonar las injurias",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/6-Perdonar-las-ofensas.png",
        },
        {
            text: "Consolar al triste",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/5-Consolar-al-triste.png",
        },
        {
            text: "Sufrir con paciencia los defectos propios y del prójimo",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/7-Soportar-con-paciencia-los-defectos-de-los-dem%C3%A1s.png",
        },
        {
            text:"Orar por los vivos y difuntos",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/3-Rogar-a-Dios-por-losvivos-y-muertos.png",
        },
        {
            text: "Dar de comer al hambriento",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/comer.png",
        },
        {
            text: "Dar de beber al sediento",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/agua.png",
        },
        {
            text: "Dar posada al peregrino",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/casa.png",
        },
        {
            text: "Vestir al desnudo",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/vestir.png",
        },
        {
            text: "Visitar al enfermo",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/enfermo.png",
        },
        {
            text: "Visitar a los encarcelados ",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/carcel.png",
        },
        {
            text: "Enterrar a los difuntos",
            image: "https://catholic-link.com/wp-content/uploads/2019/07/difunto.png",
        }
    ];

</script>

<style>
    .carrusel {
        display: flex;
        flex-wrap: nowrap;
        overflow: scroll;        
    }
    h1 {
  font-size: 4rem;
  margin-top: 0;
  margin-bottom: 80px;
}

h1 span {
  color: #17B6D2;
}
</style>
 
<div class="carrusel">

    <h1>
        Obras: <span>de misericordia</span>
      </h1>
      
    {#each positions as position}
    <Card {...position} />
    {/each}
</div>

