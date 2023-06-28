<script setup>
    definePageMeta({
        layout: "card",
    });
</script>

<template>
    <card-section class="overflow-hidden h-screen flex flex-col justify-center text-[#9b8579] bg-[#fdfbf6]">
        <div class="relative m-3 px-3 py-32 border-8 border-[#e0d4bf]">
            <img class="absolute bottom-0 right-0 w-16 translate-y-1/2 scale-[3]" src="~/assets/images/flower-1.svg" alt="Flower 1"/>
            <img class="absolute bottom-0 left-0 w-16 translate-y-1/2 scale-[4]" src="~/assets/images/flower-2.svg" alt="Flower 1"/>
            <img class="absolute top-0 right-0 w-16 translate-y-1/2 scale-[5]" src="~/assets/images/flower-3.svg" alt="Flower 1"/>
            <img class="absolute top-0 left-0 w-16 -translate-x-1/2 -translate-y-20 scale-[1.75]" src="~/assets/images/flower-4.svg" alt="Flower 1"/>
            <p class="uppercase text-lg">Majlis<br/>Perkahwinan</p>
            <div class="text-3xl text-[#b38f69] my-6">
                <p>Amirul Arif</p>
                <p class="text-center text-sm">dan</p>
                <p class="text-right">Nurul Nabila</p>
            </div>
            <p class="flex flex-row text-center justify-center mb-3">
                <span class="align-middle my-auto mx-3">Sep</span>
                <span class="align-middle mx-3 px-3 border-x-4">Sabtu<br/><span class="text-2xl">16</span></span>
                <span class="align-middle my-auto mx-3">2023</span>
            </p>
            <p class="text-center">Seksyen 27, Shah Alam, Selangor.</p>
        </div>
    </card-section>
    <card-section class="text-center text-[#9b8579] bg-[#fdfbf6]">
        <p class="tracking-widest mb-3">Assalamualaikum W.B.T</p>
        <p class="text-xl mb-3">Hj Mohd Solong Bin Abdul Ghani<br/>Hjh Noorma Binti Othman</p>
        <p class="text-xs">
            Dengan penuh kesyukuran ke hadrat Ilahi, kami sekeluarga menjemput
            <br/>
            Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh
        </p>
        <p class="text-xs mb-6">sekeluarga hadir ke Majlis Pernikahan anakanda kami</p>
        <p class="text-lg">Amirul Arif Bin Mohd Sulong</p>
        <p class="text-xs">dan</p>
        <p class="text-lg">Nurul Nabila Natasya Binti Abu Bakar</p>
    </card-section>
    <card-section class="text-center text-[#b38f69]">
        <p>Sabtu, 16 September 2023</p>
        <p class="mb-3">30 Safar 1445h</p>
        <p class="mb-3">11.30 AM - 4.00 PM</p>
        <p>No. 11, Jalan Bukit Rasa 27/81,</p>
        <p>Seksyen 27, 40400, Shah Alam,</p>
        <p>Selangor.</p>
    </card-section>
    <card-section class="text-center text-[#9b8579] bg-[#fdfbf6]">
        <p>Semoga dengan kehadiran dan doa restu</p>
        <p>Dato' / Datin / Tuan / Puan / Encik / Cik / Hj / Hjh</p>
        <p>dapat menyerikan lagi majlis kami dan diberkati Allah SWT</p>
    </card-section>
    <card-section class="text-center text-[#9b8579] bg-[#fdfbf6]">
        <p>Hubungi:</p>
        <table class="mx-auto">
            <tbody>
                <tr>
                    <td class="text-right">
                        Sulong :
                    </td>
                    <td class="text-left pl-3">
                        013 383 1228
                    </td>
                </tr>
                <tr>
                    <td class="text-right">
                        Noorma :
                    </td>
                    <td class="text-left pl-3">
                        013 219 8298
                    </td>
                </tr>
                <tr>
                    <td class="text-right">
                        Anwar :
                    </td>
                    <td class="text-left pl-3">
                        013 262 8238
                    </td>
                </tr>
                <tr>
                    <td class="text-right">
                        Naim :
                    </td>
                    <td class="text-left pl-3">
                        019 340 8298
                    </td>
                </tr>
            </tbody>
        </table>
        <p>Turut Mengundang Seisi Keluarga</p>
    </card-section>
    <card-footer />
</template>