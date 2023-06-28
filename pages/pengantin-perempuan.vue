<script setup>
    definePageMeta({
        layout: "card",
    });

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
</script>

<template>
    <card-section class="h-screen flex flex-col justify-center">
        <div class="m-3 px-3 py-32 border-8 text-center">
            <p class="uppercase text-lg">Jemputan Majlis</p>
            <p class="text-xl">Walimatul Urus</p>
            <div class="text-3xl my-12">
                <p>Nurul Nabila</p>
                <p class="text-sm">&</p>
                <p>Amirul Arif</p>
            </div>
            <p>Sabtu</p>
            <p class="flex flex-row text-center justify-center mb-3">
                <span>&nbsp;&nbsp;&nbsp;&nbsp;09</span>
                <span class="mx-3 px-3 border-x-4">September</span>
                <span>2023</span>
            </p>
            <p>Sofea Guest House<br/>Taman Bukit Dahlia, Pasir Gudang, Johor.</p>
        </div>
    </card-section>
    <card-section class="text-center">
        <p>Assalamualaikum W.B.T</p>
        <p>Abu Bakar Bin Ahmad</p>
        <p>Rafidah Binti Mohd Sharif</p>
        <p>Dengan penuh kesyukuran ke hadrat Ilahi, kami sekeluarga menjemput</p>
        <p>Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh</p>
        <p>sekeluarga hadir ke Majlis Pernikahan anakanda kami</p>
        <p>Nurul Nabila Natasya Binti Abu Bakar</p>
        <p>dan</p>
        <p>Amirul Arif Bin Mohd Sulong</p>
    </card-section>
    <card-section class="text-center">
        <p>Sabtu, 09 September 2023</p>
        <p>23 Safar 1445h</p>
        <p>11.30 Am - 4.00 Pm</p>
        <p>Sofea Guest House</p>
        <p>No 6, Jalan Dahlia 4,</p>
        <p>Taman Bukit Dahlia,</p>
        <p>81700 Pasir Gudang,</p>
        <p>Johor.</p>
    </card-section>
    <card-section class="text-center">
        <p>Semoga dengan kehadiran dan doa restu</p>
        <p>Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh</p>
        <p>dapat menyerikan lagi majlis kami dan diberkati Allah SWT</p>
    </card-section>
    <card-section class="text-center">
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
    <card-footer :contacts="contacts" :maps="maps"/>
</template>