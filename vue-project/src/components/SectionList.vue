<template>
    <SectionOverview v-for="section in sections" :section="section" />
</template>

<script setup>
import camping_1 from '@/assets/camping_1.webp'
import SectionOverview from './SectionOverview.vue'

const sections = [{
    title: 'General Information, Fees, and Parking',
    description: 'This section contains general information about the campground, including fees and parking.',
    id: 'general-information',
    parts: [
        {
            title: 'The Camping Season',
            description: 'The camping season is mid April to mid October',
            content: [
                {
                    heading: 'Variable Dates',
                    body: 'TRC’s Camping Season traditionally starts on the second Saturday of April and continues through the second Saturday of October. The dates are subject to the weather and may be earlier or later. The official opening date will be posted on TRC’s website and communicated to Site Coordinators. No camping is allowed during the remainder of the year without explicit written permission from the VP of Operations.',
                },
                {
                    heading: 'Tent Camping',
                    body: 'Tent Camping generally starts at the beginning of May and ends the last week of September. Tent camping start dates will be announced on the TRC website, Facebook, and via e-mail and are dependent on the weather and safety conditions. If the start date occurs prior to Memorial Day weekend, be advised that the trails may need to be cleared and tarps may not be up yet.',
                },
                {
                    heading: 'RV Camping',
                    body: 'RV Camping is available through the full Camping Season unless otherwise noted.',
                },
                {
                    heading: 'Seasonal Sites',
                    body: 'Seasonal Sites can begin setup as soon as the official date is announced. Minimum Occupancy requirements come into effect in mid-May and continue through Labor Day weekend.',
                },
            ],
            href: '#gen-info-a',
            id: 'gen-info-a',
            imageUrl:
                camping_1,
        },
        {
            title: 'Fees',
            description: 'The fees for the 2021 season are as follows: $195 for a regular membership, $300 for a seasonal membership, and $20 per night for RV camping.',
            content: [
                {
                    heading: 'Overnight (Limited Membership)',
                    body: 'The overnight camping fee shall be $22.00 per night for each night of camping.',
                },
                {
                    heading: 'Annual Membership',
                    body: '<ul><li>Regular Membership: $195</li><br/><li>Seasonal Membership: $300</li></ul><br/>These membershipts entitle members to unlimited camping during the regular camping season. Current camping rules apply to all members.',
                },
                {
                    heading: 'Limited Member RV Reservations',
                    body: 'Limited Member RV Reservation fees are $20 for non-members per vehicle, per night.',
                },
                {
                    heading: 'Discounted Membership',
                    body: 'TRC offers a $65 discount on annual membership fees and seasonal membership fees to senior citizens who are 65+, military veterans, members of the military, full-time students who are 21+, and people with disabilities. Documented proof of eligibility is required in order to receive this discount. <br /> <br/>Government or school-issued photo identification is acceptable proof of eligibility. Other forms of documentation may be accepted at the discretion of the Membership & Fees Committee.',
                },
                {
                    heading: 'Day Membership',
                    body: 'The day membership fee is $10. This fee allows individuals to enjoy TRC for a day and is only valid until 6:00 PM at which time they must vacate the premises. Day membership is not available during any event weekends.'
                }

            ],
            href: '#gen-info-b',
            id: 'gen-info-b',
            imageUrl:
                camping_1,
        },
        {
            title: 'Enforcement of Membership Fees for Regular Members',
            description: 'This part describes how the campground enforces membership fees for regular members.',
            content: [
                {
                    heading: 'Membership Expiration',
                    body: 'Regular and seasonal members of TRC will be notified by the Treasurer when their membership is within 30 days of expiring',
                },
                {
                    heading: '30 Days to Remedy',
                    body: 'Beginning 30 days from expiration date, until a period of 30 days after expiration, the member has the obligation to either pay the membership fee or contact the Treasurer to arrange a payment plan.',
                },
                {
                    heading: 'Repayent of Overdue fees',
                    body: 'If, for whatever reason, the Treasurer and the member are unable to reach an agreement, or the member does not wish to go through the Treasurer (PRIOR to 30-day membership lapse) the member may write to the Rules Committee for consideration. The Rules Committee will make a decision within 72 hours of a payment arrangement request from a member.',
                },
                {
                    heading: 'Camping While Fees are Expired',
                    body: 'embers that wish to camp with an expired membership must pay the limited camping fees of TRC. These fees may and will be credited towards membership dues if paid in full within 30 days.',
                },
                {
                    heading: 'Revocation of Membership',
                    body: 'If membership with TRC has lapsed for more than 30 days, the member will be removed from the list of registered members and will not be allowed to stay at TRC until fees are paid, or the member may pay limited camping fees.',
                },
                {
                    heading: 'Reinstatement of Membership',
                    body: 'To reinstate membership, the member must pay ALL their membership fees in full to become current and able to stay at TRC'
                },
            ],
            href: '#gen-info-c',
            id: 'gen-info-c',
            imageUrl:
                camping_1,
        },
        {
            title: 'Limited Campsites',
            description: 'There are a limited number of campsites available at TRC. As such, campsites are available on a first-come, first-served basis.',
            content: [
                {
                    heading: 'Stay Limit',
                    body: 'Those campsites designated as limited are intended for regular and limited members and no member may camp for any more than 14 consecutive days.'
                },
                {
                    heading: 'Cooldown Period',
                    body: 'If a member camps for 14 consecutive days, they may not stay again until 5 days have elapsed. Upon departure, any items left behind become the property of TRC.'
                },
            ],
            href: '#gen-info-d',
            id: 'gen-info-d',
            imageUrl:
                camping_1,
        },
        {
            title: 'Parking',
            description: 'Parking is available at TRC. However, parking is limited to one vehicle per campsite. If a campsite has more than one vehicle, the additional vehicles must be parked in the overflow parking area.',
            content: [
                {
                    heading: 'Parking Lot',
                    body: 'The Parking lot is reserved for TRC members on a first-come first-served basis. All vehicles are to be parked in the parking lot. Motorcycles MUST be parked in the parking lot.'
                },
                {
                    heading: 'Parking Spaces',
                    body: 'Membership does not assure parking or space for an RV. Membership applies to the person and NOT for the vehicle'
                },
                {
                    heading: 'Handicap Parking',
                    body: 'Handicap parking is reserved for those displaying a handicap sticker. During Special Events, parking permits must be visible through the front window of the vehicle.'
                },
                {
                    heading: 'Vehicle Alarms',
                    body: 'When possible, vehicle alarms MUST be deactivated while using the parking lot. Please be courteous when parking.'
                },
                {
                    heading: 'Other',
                    body: '<ul><li>! Improperly parked or abandoned vehicles will be towed at the owner’s expense. </li><br/><li>!! Speed limit throughout the campground shall be 5 mph/8 kph. </li><br/><li>!!! The combination to the gate is not to be given out to anyone who is not a Regular member of TRC.</li></ul>'
                },
                {
                    heading: 'Recreational Vehicles (RVs)',
                    body: '<ul><li>## RV Campers must use the TRC RV reservation system.</li><br/><li>## RVs in Limited camping locations must be occupied at all times.</li><br/><li>## RVs may not take additional vehicle parking and all towing vehicles must be unhooked and parked in the Vehicle Parking lot and not the RV lot.</li><br/><li>## Proof of TRC registration and payment must be displayed in the window of the RV/Trailer/Van (as well as the towing vehicle).</li><br/><li>## Grey water may not to be dumped within 50 feet of the nearest stream or riverbank.</li><br/><li>## The dumping of Black water is strictly prohibited.</li></ul>'
                },
            ],
            href: '#gen-info-e',
            id: 'gen-info-e',
            imageUrl:
                camping_1,
        },
    ]
}
]
</script>