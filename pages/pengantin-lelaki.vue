<script setup>
    definePageMeta({
        layout: "card",
        title: "Majlis Lelaki"
    })

    const calendar = {
        day: 'Sabtu',
        date: {
            masihih: '16 September 2023',
            hijrah: '30 Safar 1445H'
        },
        time: '11.30 AM - 4.00 PM',
        add: {
            gcalendar: 'https://calendar.google.com/calendar/render?action=TEMPLATE&text=Walimatul+Urus+-+Amirul+Arif+dan+Nurul+Nabila&details=Wedding&dates=20230916T110000/20230916T160000&location=11,+Jalan+Bukit+Rasa,+27/81',
            ics: '/ics/majlis_lelaki.ics',
            outlook: 'https://outlook.office.com/calendar/0/deeplink/compose?subject=Walimatul+Urus+-+Amirul+Arif+dan+Nurul+Nabila&body=Wedding&startdt=2023-09-16T11:00:00+00:00&enddt=2022-09-16T16:00:00+00:00&location=11,+Jalan+Bukit+Rasa,+27/81&path=%2Fcalendar%2Faction%2Fcompose&rru=addevent',
        }
    }

    const contacts = [
        {
            name: "Sulong",
            number: "013 383 1228"
        },
        {
            name: "Noorma",
            number: "013 219 8298"
        },
        {
            name: "Anwar",
            number: "013 262 8238"
        },
        {
            name: "Naim",
            number: "019 340 8298"
        },
    ]

    const maps = {
        iframe: 'https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3984.3196353916824!2d101.56240008463271!3d3.008433246199642!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31cdb2e3ad0eceeb%3A0x2597934088a2786a!2s11%2C%20Jalan%20Bukit%20Rasa%2027%2F81%2C%20Taman%20Bunga%20Negara%2C%2040400%20Shah%20Alam%2C%20Selangor!5e0!3m2!1sen!2smy!4v1687917749311!5m2!1sen!2smy',
        share: {
            gmap: 'https://goo.gl/maps/YeDdKSztNGHpLPQx7',
            waze: 'https://www.waze.com/en/live-map/directions/my/selangor/shah-alam/11,-jalan-bukit-rasa-2781?place=ChIJ684OreOyzTERaniiiECTlyU'
        }
    }

    const footerDetails = {
        calendar: calendar,
        contacts: contacts,
        maps: maps,
    }
</script>

<template class="bg-gray-100">
    <div>
        <card-section class="overflow-hidden flex flex-col justify-center text-groomSecondary bg-groomPrimary font-['Georgia']">
            <div class="relative m-3 px-3 py-32 border-8 border-[#e0d4bf]">
                <img class="absolute bottom-0 right-0 w-16 translate-y-1/2 scale-[3]" src="~/assets/images/flower-1.svg" alt="Flower 1"/>
                <img class="absolute bottom-0 left-0 w-16 translate-y-1/2 scale-[4]" src="~/assets/images/flower-2.svg" alt="Flower 2"/>
                <img class="absolute top-0 right-0 w-16 translate-y-1/2 scale-[5]" src="~/assets/images/flower-3.svg" alt="Flower 3"/>
                <img class="absolute top-0 left-0 w-16 -translate-x-1/2 -translate-y-20 scale-[3]" src="~/assets/images/flower-4.svg" alt="Flower 4"/>
                <p class="uppercase tracking-widest">Majlis Perkahwinan</p>
                <div class="text-3xl tracking-widest font-bold text-center text-groomTertiary my-12 font-GreatVibes">
                    <p class="sm:text-5xl">Amirul Arif</p>
                    <p class="text-sm font-['Georgia']">dan</p>
                    <p class="sm:text-5xl">Nurul Nabila</p>
                </div>
                <p class="flex flex-row text-center justify-center mb-3">
                    <span class="align-middle my-auto mx-3">Sep</span>
                    <span class="align-middle mx-3 px-3 border-x-4">Sabtu<br/><span class="text-2xl">16</span></span>
                    <span class="align-middle my-auto mx-3">2023</span>
                </p>
                <p class="text-center">Seksyen 27, Shah Alam, Selangor.</p>
            </div>
        </card-section>
        <card-section class="text-center text-groomSecondary bg-groomPrimary font-['Georgia']">
            <p class="tracking-widest mb-3">Assalamualaikum W.B.T</p>
            <p class="text-xl mb-3 font-Baskerville">Hj Mohd Solong Bin Abdul Ghani<br/>Hjh Noorma Binti Othman</p>
            <p class="text-xs">
                Dengan penuh kesyukuran ke hadrat Ilahi, kami sekeluarga menjemput
                <br/>
                Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh
            </p>
            <p class="text-xs mb-6">sekeluarga hadir ke Majlis Pernikahan anakanda kami</p>
            <p class="text-lg font-Baskerville">Amirul Arif Bin Mohd Sulong</p>
            <p class="text-xs">dan</p>
            <p class="text-lg font-Baskerville">Nurul Nabila Natasya Binti Abu Bakar</p>
        </card-section>
        <card-section class="text-center text-groomTertiary bg-white font-Baskerville">
            <p>Sabtu, 16 September 2023</p>
            <p class="mb-3">30 Safar 1445h</p>
            <p class="mb-3">11.30 AM - 4.00 PM</p>
            <p>No. 11, Jalan Bukit Rasa 27/81,</p>
            <p>Seksyen 27, 40400, Shah Alam,</p>
            <p>Selangor.</p>
        </card-section>
        <card-section class="text-center text-groomSecondary bg-groomPrimary font-Baskerville">
            <p>Semoga dengan kehadiran dan doa restu</p>
            <p>Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh</p>
            <p>dapat menyerikan lagi majlis kami dan diberkati Allah SWT</p>
        </card-section>
        <card-section class="text-center text-groomSecondary bg-groomPrimary font-Baskerville">
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
        <div class="py-1 text-xs text-white text-center bg-[#282928] border-t border-black">
            Dihasilkan oleh <a href="https://naimsolong.github.io" target="_blank" class="hover:font-bold underline">Amirul Naim</a>
        </div>
    </div>
    <card-footer :footerDetails="footerDetails"/>
</template>
