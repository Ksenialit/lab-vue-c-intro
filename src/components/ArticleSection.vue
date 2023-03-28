<template>
    <section>
        <img :src="icon" alt="article icon">
        <h2>{{ title }}</h2>
        <p> {{ description }}</p>
    </section>
</template>

<script>
export default {
    name: "ArticleSections",
    props: {
        icon: {
            type: String,
        },
        title: {
            type: String,
        },
        description: {
            type: String
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