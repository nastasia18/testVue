<template>
    <v-row>
        <v-col class="cafe__component">
            <h1 class="py-4">Lists of cafes</h1>

            <v-row class="cafe__list mx-2">
                <v-col v-for="cafe in cafes" :key="cafe.id" md="4">
                    <v-card class="cafe__card">
                        <v-img height="250" :src="cafe.img"></v-img>
                        <v-card-title>{{cafe.name}}</v-card-title>
                        <v-card-text>
                            <p>{{cafe.description}}</p>
                            <p>{{cafe.rating}}</p>
                        </v-card-text>
                    </v-card>
                </v-col>
            </v-row>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        name: 'CafeComponent',
        data: () => ({
            cafes: [
                {
                    id: 0,
                    name: 'K-FOOD',
                    description: 'lALALAL',
                    img: 'http://invest.vologda-portal.ru.srv2.place-start.ru/wp-content/uploads/2021/12/заглушка.jpg',
                    tags: ['asian'],
                    rating: 5
                },
                {
                    id: 1,
                    name: 'K-FOOD1',
                    description: 'lALALAL1',
                    img: 'http://invest.vologda-portal.ru.srv2.place-start.ru/wp-content/uploads/2021/12/заглушка.jpg',
                    tags: ['russia', '24/7'],
                    rating: 4
                },
                {
                    id: 2,
                    name: 'K-FOOD2',
                    description: 'lALALAL2',
                    img: 'http://invest.vologda-portal.ru.srv2.place-start.ru/wp-content/uploads/2021/12/заглушка.jpg',
                    tags: ['italia'],
                    rating: 5
                },
                {
                    id: 3,
                    name: 'K-FOOD3',
                    description: 'lALALAL3',
                    img: 'http://invest.vologda-portal.ru.srv2.place-start.ru/wp-content/uploads/2021/12/заглушка.jpg',
                    tags: ['russia'],
                    rating: 5
                },
                {
                    id: 4,
                    name: 'K-FOOD4',
                    description: 'lALALAL4',
                    img: 'http://invest.vologda-portal.ru.srv2.place-start.ru/wp-content/uploads/2021/12/заглушка.jpg',
                    tags: ['asian', 'chinese'],
                    rating: 4
                }
            ]
        })
    }
</script>