<template>
    <section>
        <img src="icon" alt="article icon">
        <h2>{{ title }}</h2>
        <p> {{ description }}</p>
    </section>
</template>

<script>
export default {
    name: "ArticleSections",
    props: { 
        data() {
            return {
                items: [
                { image:'',
                title: 'Performant',
                text: 'Truly reactive, compiler-optimized rendering system that rarely requires manual optimization.'}, 
                { image:'',
                title: 'Approachable',
                text: 'Builds on top of standard HTML, CSS and JavaScript with intuitive API and world-class documentation.'}, 
                { image:'',
                title: 'Versatile',
                text: 'A rich, incrementally adoptable ecosystem that scales between a library and a full-featured framework.'}, 
                ]
            }
        }
    }
}


</script>

<style scoped>
    section {
        display: flex;
        justify-content: center;
        flex-direction: column;
    }

    img {
        width: 60px;
        height: 60px;
    }

    h2 {
        font-family: 'Inter';
        font-style: normal;
        font-weight: 700;
        font-size: 16px;
        line-height: 95px;
        text-align: center;
        letter-spacing: -0.02em;
        color: #000000;
    }

    p {
        font-family: 'Inria Sans';
        font-style: normal;
        font-weight: 400;
        font-size: 12px;
        line-height: 17px;
        text-align: center;
        letter-spacing: -0.02em;
        color: #000000;
    }
</style>