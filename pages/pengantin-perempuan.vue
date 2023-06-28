<script setup>
    definePageMeta({
        layout: "card",
    })

    const backgroundUrl = '/pattern-1.png'

    const calendar = {
        day: 'Sabtu',
        date: {
            masihih: '09 September 2023',
            hijrah: '23 Safar 1445H'
        },
        time: '11.30 AM - 4.00 PM'
    }

    const contacts = [
        {
            name: "Abu Bakar",
            number: "018 665 3059"
        },
        {
            name: "Rafidah",
            number: "011 5754 2732"
        },
        {
            name: "Hariz",
            number: "018 222 0431"
        },
        {
            name: "Kamarul",
            number: "018 662 3321"
        },
    ]
    
    const maps = {
        iframe: 'https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.49464470501!2d103.89758217582393!3d1.47592356115587!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31da15b9e1f24c5b%3A0xc075eeb910947d1f!2sSofea%20Guest%20House!5e0!3m2!1sen!2smy!4v1687918092406!5m2!1sen!2smy',
        share: {
            gmap: 'https://goo.gl/maps/evGAnusEnCFHbZC9A',
            waze: 'https://www.waze.com/en/live-map/directions/my/johor/pasir-gudang/sofea-guest-house?place=ChIJW0zy4bkV2jERH32UELnudcA'
        }
    }

    const footerDetails = {
        calendar: calendar,
        contacts: contacts,
        maps: maps,
    }
</script>

<template>
    <card-section class="overflow-hidden h-screen flex flex-col justify-center text-brideSecondary bg-white" :style="{ backgroundRepeat: repeat, backgroundImage: `url(${backgroundUrl})` }">
        <div class="relative m-3 px-3 py-32 text-center">
            <div class="absolute top-0 left-0 w-full h-full border-8 border-white drop-shadow-xl"></div>
            <img class="absolute bottom-0 right-0 w-16 -translate-x-1/2 -translate-y-1/2 scale-[4]" src="~/assets/images/flower-8.svg" alt="Flower 8"/>
            <img class="absolute bottom-0 left-0 w-16 translate-x-1/2 -translate-y-1/2 scale-[4]" src="~/assets/images/flower-6.svg" alt="Flower 6"/>
            <img class="absolute top-0 right-0 w-16 -translate-x-1/2 translate-y-1/2 scale-[5]" src="~/assets/images/flower-7.svg" alt="Flower 7"/>
            <img class="absolute top-0 left-0 w-16 translate-x-1/2 scale-[4]" src="~/assets/images/flower-5.svg" alt="Flower 5"/>
            <p class="uppercase text-lg text-brideTertiary">Jemputan Majlis</p>
            <p class="text-xl text-brideTertiary">Walimatul Urus</p>
            <div class="text-3xl my-12">
                <p>Nurul Nabila</p>
                <p class="text-sm">&</p>
                <p>Amirul Arif</p>
            </div>
            <p class="text-brideTertiary">Sabtu</p>
            <p class="flex flex-row text-center justify-center mb-3 text-brideTertiary">
                <span>&nbsp;&nbsp;&nbsp;&nbsp;09</span>
                <span class="mx-3 px-3 border-x-4">September</span>
                <span>2023</span>
            </p>
            <p>Sofea Guest House<br/>Taman Bukit Dahlia, Pasir Gudang, Johor.</p>
        </div>
    </card-section>
    <card-section class="text-center text-brideSecondary bg-white" :style="{ backgroundRepeat: repeat, backgroundImage: `url(${backgroundUrl})` }">
        <p class="tracking-widest mb-3">Assalamualaikum W.B.T</p>
        <p class="text-xl mb-3">Abu Bakar Bin Ahmad<br/>Rafidah Binti Mohd Sharif</p>
        <p class="text-xs">
            Dengan penuh kesyukuran ke hadrat Ilahi, kami sekeluarga menjemput
            <br/>
            Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh
        </p>
        <p class="text-xs mb-6">sekeluarga hadir ke Majlis Pernikahan anakanda kami</p>
        <p class="text-lg">Nurul Nabila Natasya Binti Abu Bakar</p>
        <p class="text-xs">dan</p>
        <p class="text-lg">Amirul Arif Bin Mohd Sulong</p>
    </card-section>
    <card-section class="text-center text-brideTertiary bg-white">
        <p>Sabtu, 09 September 2023</p>
        <p class="mb-3">23 Safar 1445h</p>
        <p class="mb-3">11.30 AM - 4.00 PM</p>
        <p>Sofea Guest House</p>
        <p>No 6, Jalan Dahlia 4,</p>
        <p>Taman Bukit Dahlia, 81700 Pasir Gudang,</p>
        <p>Johor.</p>
    </card-section>
    <card-section class="text-center text-brideSecondary bg-white" :style="{ backgroundRepeat: repeat, backgroundImage: `url(${backgroundUrl})` }">
        <p>Semoga dengan kehadiran dan doa restu</p>
        <p>Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh</p>
        <p>dapat menyerikan lagi majlis kami dan diberkati Allah SWT</p>
    </card-section>
    <card-section class="mb-24 text-center text-brideSecondary bg-white" :style="{ backgroundRepeat: repeat, backgroundImage: `url(${backgroundUrl})` }">
        <p>Hubungi:</p>
        <table class="mx-auto">
            <tbody>
                <tr v-for="contact in contacts">
                    <td class="text-right">
                        {{ contact.name }} :
                    </td>
                    <td class="text-left pl-3">
                        {{ contact.number }}
                    </td>
                </tr>
            </tbody>
        </table>
        <p>Turut Mengundang Seisi Keluarga</p>
    </card-section>
    <card-footer :footerDetails="footerDetails"/>
</template>
