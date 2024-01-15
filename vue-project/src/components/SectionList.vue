<template>
    <SectionOverview v-for="section in sections" :section="section" />
</template>

<script setup>
import camping_1 from '@/assets/camping_1.webp'
import SectionOverview from './SectionOverview.vue'

const sections = [
    {
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
    },
    {
        title: 'TRC Standing Rules',
        description: 'This section contains the standing rules of the campground. These rules are applicable to ALL campers.',
        id: 'rules',
        parts: [
            {
                title: 'Drugs and Alcohol',
                description: 'This part describes the rules regarding drugs and alcohol at the campground.',
                content: [
                    {
                        heading: 'Buying or Selling Illegal Drugs',
                        body: 'Persons caught selling or buying drugs on TRC property will have their membership immediately terminated and will be evicted from the campground.'
                    },
                    {
                        heading: 'Over-service of Alcohol',
                        body: '<ul><li>The over serving of guests at a site may be viewed as a complicit action in any finding of a subsequent rule violation.</li><br/><li>In situations where site coordinators and/or servers over serve, either may be found in violation of the rules, even if there is no allegation of a rule violation.</li></ul>'
                    },
                    {
                        heading: 'Rowdy and Drunken Behavior',
                        body: 'Rowdy and drunken behavior will not be tolerated.'
                    },
                    {
                        heading: 'Drinking and Driving',
                        body: 'Do NOT drink and drive.'
                    },
                ],
                href: '#rules-a',
                id: 'rules-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Firearms, Weapons, and Fireworks',
                description: 'This part describes the rules regarding firearms, weapons, and fireworks at the campground.',
                content: [
                    {
                        heading: 'Firearms',
                        body: 'Firearms are not permitted on TRC property. This is considered a critical violation and may result in revocation of membership and ban from TRC property.'
                    },
                    {
                        heading: 'Weapons',
                        body: 'Weapons are not permitted on TRC property. This is considered a critical violation and may result in revocation of membership and ban from TRC property.'
                    },
                    {
                        heading: 'Fireworks',
                        body: 'Fireworks are not permitted on TRC property. This is considered a critical violation and may result in revocation of membership and ban from TRC property.'
                    },
                ],
                href: '#rules-b',
                id: 'rules-b',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Fire Safety',
                description: 'This part describes the rules regarding fire safety at the campground.',
                content: [
                    {
                        heading: 'General Rules',
                        body: '',
                        list: [
                            'All campfires must be confined to the existing designated Community Fire Pits in the lower campground or in a Fire Marshall approved fire pit in the upper campground.',
                            'Do not make a new fire pit.',
                            'Do not leave campfires unattended.',
                            'Fires must be fully extinguished before leaving.',
                            'Do not use gasoline products as fire starters.',
                            'Candles may only be burned in non-combustible containers.',
                            'The use of Tiki torches or other device utilizing flammable oil is prohibited on TRC property.',
                            'Fires must be contained in such a way that surrounding brush and trees are not affected.',
                            'No smoking in the toilets, when smoking on the trails, please use the butt cans. Please observe the fire signs and obey the no smoking on trails rule when in affect. No straw allowed in campsites.',
                        ]
                    },
                    {
                        heading: 'Fire Pits',
                        body: '<ul><li>No fire pit may be moved without permission of a TRC Fire Marshall.</li><br/><li>No campfires may be lit in a new, moved or renovated fire pit until it has been approved by the TRC Fire Marshall.</li><br/><li>Fire pits must be located, and fires contained, in such a way that surrounding brush and trees are not affected</li></ul>'
                    },
                    {
                        heading: 'Fire Protection',
                        body: '<ul><li>All seasonal campsites shall maintain one 5-gallon covered water pail at the entrance to their site and another near their fire pit.</li><br/><li>All Limited sites are provided with one 5-gallon covered water pail near their respective fire pits and members shall ensure they are full at all times.</li><br/><li>All sites that include a dining area shall maintain one or more ABC type fire extinguisher(s) totaling at least 10 pounds.</li><br/><li>All sites must agree to periodic inspections by the TRC Fire Marshall(s) and will comply with their recommendations.</li></ul>'
                    },
                    {
                        heading: 'Fire Suppresion System',
                        body: 'The water provided by the shared fire suppression system is not for consumption and shall not to be used for drinking, washing, or any other purpose other than emergency fire suppression situations.'
                    },
                ],
                href: '#rules-c',
                id: 'rules-c',
                imageUrl:
                    camping_1,
            },
            {
                title: 'General Rules',
                description: 'This part describes the general rules of the campground.',
                content: [
                    {
                        heading: 'Pets',
                        body: '',
                        list: [
                            'The control of pets is the sole responsibility of the member at all times.',
                            'Pick up after your pets and dispose of the waste into the garbage not the honey buckets or butt cans. ',
                            'Dogs must be on a leash when on TRC trails.'
                        ]
                    },
                    {
                        heading: 'Garbage',
                        body: '',
                        list: [
                            'TRC provides limited garbage service for members only, limited to regular household kitchen type refuse. No building materials; furniture; appliances; or camping gear of any kind may be dumped in the bins.',
                            'Hazardous waste includes, but is not limited to, marine and deep cycle batteries, florescent lights and paint products. If you have recycling at home, please help the environment and take these items home. A $500 fine will be imposed for anyone putting hazardous material in the dumpsters'
                        ]
                    },
                    {
                        heading: 'Noise Abatement',
                        body: '',
                        list: [
                            'No loud noise allowed between 10 PM and 9 AM that affects your immediate neighbors. Members, please be considerate of your neighbors. Exceptions to this rule are during TRC organized/approved party or social activity areas.',
                            'Vehicles shall not be driven on trails 5 and 6 between 12 midnight and 9 AM.'
                        ]
                    },
                    {
                        heading: 'Nudity',
                        body: 'TRC is a clothing optional campground, with the following exceptions:',
                        list: [
                            'No nudity or sexual acts in the parking lot, on the highway, or visible to river travelers and/or TRC neighbors.'
                        ]
                    },
                    {
                        heading: 'Beach',
                        body: 'No fires or glass containers are allowed on the beach. Please use the provided butt cans for butts only and carry out all other garbage. Pick up after your pets'
                    },
                    {
                        heading: 'Wheelbarrows',
                        body: 'TRC supplied wheelbarrows are to be used to move provisions, supplies and equipment from a vehicle to a campsite. They are for limited time usage and must be returned to the designated area. No wheeled vehicles allowed on trails or in camping areas except wheelbarrows. No wheelbarrows on or crossing the Mountain Loop Highway'
                    },
                    {
                        heading: 'Portable Toilets',
                        body: 'Put nothing in the portable toilets but human waste. No smoking is allowed in them. No garbage, cans, bottles, cigarette butts, or any other items.'
                    },
                    {
                        heading: 'Gray and Black Water',
                        body: '',
                        list: [
                            'Black water may not be dumped anywhere on TRC property and is to be disposed of in accordance with county and state laws.',
                            'Gray water is to be disposed of appropriately and never dumped within 50 feet of the nearest stream or riverbank.',
                        ]
                    },
                    {
                        heading: 'Parties and Social Activities',
                        body: '',
                        list: [
                            'Camp-wide parties must be approved in advance by the TRC vice presidents in conjunction with associated or designated committees.',
                            'Party hosts are responsible for arranging for cleanup of all party litter.',
                        ]
                    },
                    {
                        heading: 'Policy on Tips, Gratuities, and Donations',
                        body: '',
                        list: [
                            'Receptacles for the purpose of collecting tips, gratuities & donations are expressly prohibited.',
                            'Private donations to individuals to cover costs shall be allowed.',
                            'Monies left to staff volunteering at a TRC event must be given to the designated Board member in charge of said event. The monies will then be delivered to the Treasurer or their designee as soon as possible.',
                        ]
                    },
                    {
                        heading: 'Pools and Water Collection',
                        body: 'Keeping with the idea of conservation of resources, the following rules shall apply to the collection of water by members:',
                        list: [
                            'Collection of water in sealed holding tanks by seasonal sites and fire suppression is permitted.',
                            'Any device used for the collection of water for decorative purposes larger than a common bird bath, shall require approval from the VP of Development.',
                            'Pools, hot tubs, and the like, are prohibited. Any questions or concerns about this shall fall under VP of Development.',
                        ]
                    },
                    {
                        heading: 'TREES',
                        body: '',
                        list: [
                            'Standing Trees – Cut no standing trees, dead or alive. No nails, screws, staples or objects of any kind may be inserted into a tree. Cables or chains attached to a tree must have a rubber or wood cushion between them and the tree.',
                            'Dangerous Trees: Notify the Tree Committee to obtain written permission to remove leaning or damaged trees that pose a danger to the safety of our members',
                        ]
                    },
                ],
                href: '#rules-d',
                id: 'rules-d',
                imageUrl:
                    camping_1,
            },
        ]
    },
    {
        title: 'Photography and Video Recording',
        description: 'This section contains the rules regarding photography and video recording at the campground.',
        id: 'photography',
        parts: [
            {
                title: 'Expectation of Privacy',
                description: 'This part describes the rules regarding photography and video recording at the campground.',
                content: [
                    {
                        heading: 'Expectation of Privacy',
                        body: '',
                        list: [
                            'TRC has been set up as a safe place for all those that wish to be safe and anonymous from the outside world. To that end, there is a reasonable expectation of privacy when members are on site; privacy to the extent that their image will not be recorded in any fashion unless they have given their permission.',
                            'Only take photographs or video recordings of members with their permission. While it is recognized that camp property does not include the beach, please be respectful at the beach as well, and consider asking before recording someone’s image.',
                        ]
                    },
                ],
                href: '#photography-a',
                id: 'photography-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Rules Pertaining to Drones, unmaned aircraft, photos, and video',
                description: 'This part describes the rules regarding drones, unmaned aircraft, photos, and video at the campground.',
                content: [
                    {
                        heading: 'Drones',
                        body: '',
                        list: [
                            'Drones, or any unmanned aircraft, are strictly prohibited, unless explicit, written permission from the VP of Operations is granted.',
                            'Drones and unmanned aircraft are not permitted to be flown in parking areas, because of the potential liability to the camp by someone who damages another member’s property.',
                            'Drones and unmanned aircraft will not be allowed to be transported to the beach areas via camp property unless you have been granted special, written permission from the VP of Operations.',
                        ]
                    },
                    {
                        heading: 'Video and Photography',
                        body: '',
                        list: [
                            'Video recording of any member without their written permission is strictly prohibited.',
                            'Images posted on social media must have written consent of those in the photographs.',
                            'Large group pictures used for the purpose of marketing shall be free of facial identification unless VP of Marketing receives written consent from those in the photo.',
                            'Pictures and video taken for the purpose of rule violations, policy violations, and criminal activity, do not pertain to this section. Posting of these violations on social media is the exclusive right of the Executive Committee.',
                        ]
                    },
                ],
                href: '#photography-b',
                id: 'photography-b',
                imageUrl:
                    camping_1,
            },
        ]
    },
]
</script>