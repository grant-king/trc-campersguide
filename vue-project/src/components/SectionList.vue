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
    {
        title: 'Campground Maintenance and Wildlife Habitat Enhancement',
        description: 'This section contains the rules regarding campground maintenance and wildlife habitat enhancement at the campground.',
        id: 'campground',
        parts: [
            {
                title: 'Policy Purpose, Scope, and Background',
                description: 'This part describes the purpose, scope, and background of the policy.',
                content: [
                    {
                        heading: 'Purpose',
                        body: 'Adopt a policy of leaving some fallen, or damaged but standing tree snags to decay in order to provide habitat for insects, birds, small mammals, and amphibians. To do so, we will need to identify areas of the campground in which to leave damaged and fallen trees for this purpose.',
                    },
                    {
                        heading: 'Scope',
                        body: 'This Policy Proposal is meant only to address issues surrounding the removal of fallen and damaged trees. Existing healthy trees anywhere on the campgrounds are to be left untouched in accordance with our Standing Rules.',
                    },
                    {
                        heading: 'Background',
                        body: 'riangle Recreation Camp suffers yearly winter damage to trees (primarily older alders) requiring significant effort to clear. This policy would limit the work required to clean up weather-damaged trees and at the same time provide enhanced habitat to certain wildlife as required in our Conditional Use Permit.',
                    },
                ],
                href: '#campground-a',
                id: 'campground-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Proposal',
                description: 'This part describes the wildlife habitat enhancement proposal.',
                content: [
                    {
                        heading: 'Policy Proposal',
                        body: '',
                        list: [
                            'Given that the purpose of our organization is to provide a safe and enjoyable outdoor environment for our members and guests, any damaged trees that pose a threat to the safety of our members and guests should be removed or rendered harmless in a manner consistent with TRC guidelines.',
                            'Given that a significant portion of our property is already designated NGPA (Native Growth Protection Area) and therefore not available for normal camping activities, it is appropriate to limit damaged tree removal in those areas in order to provide enhanced habitat for small wildlife.',
                        ]
                    },
                ],
                href: '#campground-b',
                id: 'campground-b',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Guidelines for Non-NPGA Areas',
                description: 'This part describes the guidelines for non-NPGA areas.',
                content: [
                    {
                        heading: 'Non-NPGA Area Guidelines',
                        body: '',
                        list: [
                            'Campground areas that are freely available for normal camping activity should be cleared of fallen and damaged trees in a manner suitable to our needs. This includes ensuring trails are kept clear, safe and passable, common areas are clear and safe for use, and campsites are safe and accessible.',
                            'The logs resulting from this maintenance will be disposed of or used for the benefit of our membership (e.g. firewood) as the Board of Directors sees fit by their own action or delegation to a Committee.',
                        ]
                    },
                ],
                href: '#campground-c',
                id: 'campground-c',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Guidelines for NGPA Areas',
                description: 'This part describes the guidelines for NGPA areas.',
                content: [
                    {
                        heading: 'NGPA Area Guidelines',
                        body: '',
                        list: [
                            'Fallen trees which lie entirely within an NGPA area should be left in place to provide habitat and help limit foot traffic within the restricted area except where the accumulation of those falls may pose a fire hazard.',
                            'Damaged trees (‘Leaners’) should be rendered harmless by cutting at a height that would leave a snag (stump) which, if it later fell over, would fall entirely within the NGPA area.',
                            'The logs resulting from this maintenance will be disposed of or used for the benefit of our membership (e.g. firewood) as the Board of Directors sees fit by their own action or delegation to a Committee.',
                        ]
                    },
                ],
                href: '#campground-d',
                id: 'campground-d',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Additional Habitat Enhancement',
                description: 'Members are encouraged to provide additional nesting boxes for birds, bats or small mammals in accordance with State and County standards',
                content: [
                    {
                        heading: 'Ask a Board Member for more information about this.',
                        body: '',
                        list: [
                            '',
                        ]
                    },
                ],
                href: '#campground-e',
                id: 'campground-e',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Nuisance Animals',
                description: 'Limit damage caused by opportunistic animals such as raccoons and bears.',
                content: [
                    {
                        heading: 'Harm Reduction',
                        body: 'Members are encouraged to limit damage to their property caused by opportunistic wildlife by:',
                        list: [
                            'i. Securely storing food in lockable containers.',
                            'ii. Cleaning dishes and cooking surfaces (BBQs) after meals.',
                            'iii. Not keeping garbage in their site over-night.',
                        ]
                    },
                    {
                        heading: 'Additional Measures',
                        body: 'Campsites which follow these guidelines and continue to suffer damage due to persistent nuisance animals (e.g. raccoons) should approach a member of the Executive Committee to discuss arrangements for the humane capture and removal of said animals from the campgrounds.',

                    },
                ],
                href: '#campground-f',
                id: 'campground-f',
                imageUrl:
                    camping_1,
            },
        ]
    },
    {
        title: 'Rules Violations and Internal Dispute Resolution',
        description: 'This section contains the rules regarding rules violations and internal dispute resolution at the campground.',
        id: 'violations',
        parts: [
            {
                title: 'Rule Violations',
                description: 'This part describes the procedure for handling rule violations.',
                content: [
                    {
                        heading: 'Major Violations',
                        body: 'Any member who violates the Bylaws, Rules or Regulations of TRC, local, state or federal law may have their membership immediately terminated (and be asked to leave the property). Critical violations include, but are not limited to:',
                        list: [
                            '!! Violent acts or verbal threats against other members, their guests, their property and neighboring property owners.',
                            '!! Taking or using items without permission (aka theft), or possession of stolen items.',
                            '!! Verifiable use or sale of illegal drugs on TRC property.',
                            'Illegal is defined as those substances prohibited by State or Federal law, with State laws taking precedence when applicable (e.g. cannabis)',
                            'Violators may also be subject to Criminal and or Civil prosecution.',
                        ]
                    },
                    {
                        heading: 'Rules Infractions Requiring Disciplinary Action',
                        body: '',
                        list: [
                            'All other rule infractions requiring disciplinary action shall be forwarded to the VP of Member Relations or Rules Committee for investigation and deliberation. Consequences not involving the termination or suspension of membership shall be handed down by the Rules Committee. If the Rules Committee recommends that termination or suspension of membership is appropriate, the matter shall be presented to the Board of Directors by the VP of Member Relations for discussion and vote.',
                            'The Rules Committee shall be a continuous, year-round committee. The Chair of the Committee shall be the VP of Member Relations, per the bylaws.',
                        ]
                    },
                ],
                href: '#violations-a',
                id: 'violations-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Internal Dispute Resolution',
                description: 'This part describes the procedure for handling internal disputes.',
                content: [
                    {
                        heading: 'Self-Resolution',
                        body: ' Disputes arising internally among members of a campsite are expected to be resolved by those members without involving TRC or its officers',
                        list: [
                            '',
                            '',
                            '',
                        ]
                    },
                    {
                        heading: 'Elevated Resolution',
                        body: 'Any disputes arising from the aforementioned conditions, that cannot be resolved between the parties involved shall, in the following order, present their issue in writing, for consideration to the:',
                        list: [
                            'i. Seasonal Site Committee',
                            'ii. Rules Committee',
                            'iii. Vice President the issue falls under',
                            'iv. Executive Committee for private matters of health, finance, etc.',
                            'v. Board of Directors',
                        ]
                    },
                ],
                href: '#violations-b',
                id: 'violations-b',
                imageUrl:
                    camping_1,
            },
        ]
    },
    {
        title: 'General Steps of Consequence',
        description: 'This section outlines the general steps of consequence for rules violations.',
        id: 'consequence',
        parts: [
            {
                title: 'Infractions',
                description: 'Using the "Laws of Common Sense" - Definitions',
                content: [
                    {
                        heading: 'Minor Infractions',
                        body: '',
                        list: [
                            'Minor violations of the rules may be considered as a “First Strike”. One to two committee members may investigate as deemed necessary by the Rules Committee, and the Member will be issued a verbal or written warning, which will be documented by the Rules Committee.',
                            'Said member may, depending on the nature of the violation, be placed on Probation. Probation does not jeopardize Membership status but will be taken into account if any subsequent violations occur. Probation will be lifted at the end of the Season in which the violation occurred if no further violations occur, or upon recommendation of the Rules Committee with Board approval.',
                        ]
                    },
                    {
                        heading: 'Major Infractions',
                        body: '',
                        list: [
                            'Any subsequent violations while on probation, or any single, more serious violations of the rules will be considered a “Second Strike”.',
                            'Suspension of membership status for a period of time recommended by the Rules committee may be imposed and the member’s voting rights at the Annual General Meeting may be suspended.',
                        ]
                    },
                    {
                        heading: 'Critical Infractions',
                        body: '',
                        list: [
                            'Any illegal activity (i.e. fireworks, firearms, theft, or violence) or continued violations of the rules while on probation, may be considered a “Third Strike”.',
                            'A 1-year suspension or permanent termination of one’s membership is a likely course of action. Board involvement will be necessary to approve any recommendation of suspension.',
                            'In rare situations where members are requested to leave immediately, this must be communicated to the Executive committee as soon as possible.',
                            'Would most likely begin with an immediate suspension of a membership through Executive action during the investigation and until the next scheduled BOD meeting.',
                        ]
                    },
                ],
                href: '#consequence-a',
                id: 'consequence-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Policy for Infractions',
                description: 'The following is TRC policy on how rule infractions are to be documented and handled in conjunction with the Vice President of Member Relations and the Rules Committee, unless already defined by existing rules.',
                content: [
                    {
                        heading: 'Adaptable Procedure',
                        body: 'Since every infraction varies in severity and circumstance, the following process may not be appropriate in certain situations.',
                        list: [
                            '1. The infraction is met with a verbal warning by either the VP or Director on Duty or a Rules Committee member at behest of the VP. It shall be documented by the Rules Committee, in as much detail as possible.',
                            '2. A second infraction or series of minor, documented incidents will be considered a “First Strike”. The Process of Investigation shall be followed as outlined in the following Section and the findings will either be hand delivered, emailed, or sent via USPS and documented by the Rules Committee.',
                            '3. A third rule violation by the same member will constitute a “Second Strike”. The Process of Investigation shall be followed and the findings will either be hand delivered, emailed, or sent via USPS. This shall require said member to be called before the rule committee for discussion of continued infractions. Within fifteen (15) days, the Rules Committee, in conjunction with the Vice President of Operations, will inform the member in writing, of the repercussions due to their continuing violation of TRC Rules and Policies. This report will also be presented to th Board of Directors at the next official Board meeting.',
                            '4. All infractions that result in any punitive action shall be reported to the Board at the next meeting. If the Board does not object to the recommendations presented, the recommendations shall be considered approved. Otherwise the Board may vote to vacate the recommendations or amend them by way a vote.',
                            '5. If the member wishes to appeal the decision of the Rules Committee, they may do so following the Appeals process of TRC.',
                        ]
                    },
                ],
                href: '#consequence-b',
                id: 'consequence-b',
                imageUrl:
                    camping_1,
            },
            {
                title: 'The Process of Investigation by the Rules Committee',
                description: 'This part describes the process of investigation by the Rules Committee.',
                content: [
                    {
                        heading: 'Choosing the Investigator',
                        body: '',
                        list: [
                            'The VP of Member Relations will select a member(s) of the Rules Committee that can preserve impartiality throughout the investigation, taking into account relationships to those being investigated.',
                            'Rules will note the availability of the committee members so that the investigation is done in a quick and speedy manner.',
                            'Any Rules committee member will recuse themselves from discussion if a clear conflict of interest presents itself, with the exception of procedural questions.',
                            'If no member of the Rules committee is deemed to be able to maintain impartiality, the chair may ask another regular or seasonal member to assist at their discretion.',
                        ]
                    },
                    {
                        heading: 'Investigation Process',
                        body: '',
                        list: [
                            'The incident report will be communicated to the Rules committee for discussion either in person or via electronic means as soon as possible.',
                            'The Chair will choose those that will lead the investigation, as outlined in the previous section.',
                            'Investigators will interview all parties involved, including the VP under which the violation falls.',
                            'The Rules Committee will meet after the investigators have handed in reports to the chair and discuss.',
                            'The chair of the Rules Committee will submit their findings and proposed recommendation of consequences in writing to the member in question and notify them of the time and location of the upcoming Board meeting where the incident will be discussed and any objections to the recommendations by the Board may discussed and voted on, if necessary. ',
                            'The chair of the Rules Committee will also provide the incident report and the committee’s recommendation to the BOD at the next scheduled BOD meeting. The member in question is strongly encouraged to attend.',
                            'If the member in question is not satisfied with the findings of The Rules Committee or vote, they have the right to follow the Grievance and Appeals process as stated in the following part.',
                        ]
                    },
                ],
                href: '#consequence-c',
                id: 'consequence-c',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Coplaint/Grievance & Appeals Policy',
                description: 'This part describes the general policies for filing complaints or an appealing a board decision.',
                content: [
                    {
                        heading: 'Concerns regarding incidents on TRC property or while conducting business for or with TRC',
                        body: '',
                        list: [
                            'Any TRC Member may raise a concern regarding their personal experience while on TRC grounds and /or conducting TRC business. This would typically include cases where there is illegal activity, dangerous situations, rules infractions, etc. Anytime you feel you were treated in an unprofessional way, or a decision was made that you feel was inconsistent with the facts.',
                            'Members are encouraged to discuss the matter first directly with the person(s) involved. If that is not satisfactory, or not possible, you are encouraged to submit an incident report for review by the Rules Committee',
                        ]
                    },
                    {
                        heading: 'Reporting Incidents',
                        body: 'It is highly recommended that all incidents of illegal activity and/or dangerous situations be reported immediately.',
                    },
                    {
                        heading: 'Filing an Incident Report',
                        body: '',
                        list: [
                            'TRC incident report forms are available in the phone kiosk during the regular camping season.E - copies are also available year - round online on the TRC website pages under “files”.',
                            'Members should complete an incident report form ASAP after the incident occurs.Once completed it should be submitted to the VP of Member Relations, or any other Executive Committee member, to be forwarded to the Rules Committee for investigation.Keeping a copy for your records is recommended.',
                            'The Rules Committee shall respond in writing within 15 days during the regular camping season, and 30 days during the off season.',
                            'When filing a report, please clearly reference which rules have been alleged to have been violated, along with as much detail as possible.Including names, sites, etc',
                        ]
                    },
                    {
                        heading: 'Appealing a Decision',
                        body: '',
                        list: [
                            'If the Member does not agree with the decision of the Rules Committee, they may appeal by completing the member complaint form attached to the Rules Committee’s written response and submit it to the Executive Committee for review.',
                            'The Executive Committee shall respond in writing within 15 days during the regular camping season, and 30 days during the off season.',
                            'If the member does not agree with the decision of the Executive Committee, they may appeal by completing the member grievance form attached to the Executive Committee’s written response and submitting it to the TRC Board of Directors for review.',
                            'The Board of Directors shall respond in writing within 45 days during the regular camping season and within 45 days following the first regular Board of Directors Meeting if submitted during the off season.',
                            'The TRC Secretary shall send a letter to the member(s) who had the concern/complaint regarding the final decision of the Board.',
                        ]
                    },
                ],
                href: '#consequence-d',
                id: 'consequence-d',
                imageUrl:
                    camping_1,
            },
        ]
    },
    {
        title: 'Seasonal Camping',
        description: 'This section contains the',
        id: 'seasonal-camping',
        parts: [
            {
                title: 'Seasonal Sites Committee',
                description: 'This part describes the purpose of the Seasonal Sites Committee.',
                content: [
                    {
                        heading: 'Overview',
                        body: 'The Seasonal Site Committee’s purpose is to oversee the administration of Seasonal Sites at TRC. This is a standing committee organized under the VP of Operations, and members are appointed by the board of directors. The committee has the authority to add or remove members during the year.',
                        list: [
                            '',
                            '',
                        ]
                    },
                    {
                        heading: 'Purpose',
                        body: '',
                        list: [
                            'To maintain a waiting list of members who want to join an existing or occupy an available Seasonal Site.',
                            'To approve new members of Seasonal Sites subject to application and approval by the Committee. ',
                            'To create and maintain a guide of best practices for Seasonal Sites to be provided to Seasonal Site coordinators prior to the beginning of camping season.',
                            'To help resolve unsettled disputes between members of Seasonal Sites.',
                        ]
                    },
                    {
                        heading: 'Scope',
                        body: 'The Seasonal Site Committee will only assist in Seasonal Site affairs when it deems it absolutely necessary. Serious issues may be referred to the Rules Committee, depending on the severity of the situation. ',
                    },
                ],
                href: '#seasonal-camping-a',
                id: 'seasonal-camping-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Sites',
                description: 'This part describes seasonal site availability, the waiting list, site assignment, and adding new members to Seasonal Sites.',
                content: [
                    {
                        heading: 'Limited Availability',
                        body: 'TRC has established a limited number of campsites on our property north of the highway designated as “Seasonal”. They are intended to be occupied by Regular members in good standing who will be camping frequently throughout the season and who agrees to maintain the site and abide by all the Conditions of Occupancy.',
                    },
                    {
                        heading: 'Application & Wait List',
                        body: 'The waiting list includes those who are approved to be offered a vacant Seasonal Site when available. Seasonal Sites become available when:',
                        list: [
                            '▪ All previous members vacate or are removed from the site.',
                            '▪ A Site has been deemed abandoned per the Abandonment process.',
                            '▪ Any other reason a site has no current members',
                            'To be added to the waiting list, the Member must be a Regular or Seasonal Member in good standing, with all fees paid in full ',
                            'Anyone wishing to be added to the waiting list must contact the Chair of the Seasonal Site Committee',
                        ]
                    },
                    {
                        heading: 'Assignment of Sites',
                        body: '',
                        list: [
                            'Assignment of a site in no way confers Ownership of that portion of TRC’s property to the members granted Occupancy. All development of the site is to be done at the assigned member’s own risk, expense and in accordance with the Development Committee’s approval. ',
                            'Upon acceptance of the Application for Occupancy, the applicants will register their campsite name, site members, and select a Site Coordinator through whom all future TRC business will be conducted. All registered members are to provide contact information (email) and sign the registration document agreeing to abide by all of TRC’s Bylaws, Standing Rules and Conditions of Occupancy.',
                            'At the termination of occupancy (either by their own or TRC’s initiative) the assigned members are responsible for the removal of all debris, structures, or improvements. Any property, approved structures, or improvements left behind after a reasonable period granted for their removal will become an integral part of that site for use by the next occupants at their discretion.',
                        ]
                    },
                    {
                        heading: 'Adding New Members to existing Seasonal Sites',
                        body: '',
                        list: [
                            'A Seasonal Site Membership Application must be completed by both the applicant and the Site Coordinator.',
                            'The Site Coordinator must submit the application to the committee chair to request the approval of the addition of the new member to their site',
                            'The Committee will review the application and inform the Site Coordinator of their decision. If approved, the applicant shall be considered a Seasonal Conditional Member, subject to the conditions outlined in this Guide.',
                            'Any Committee decisions may be appealed according to the appeals process outlined in the Campers Guide. ',
                        ]
                    },
                ],
                href: '#seasonal-camping-b',
                id: 'seasonal-camping-b',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Conditions of Occupancy for Seasonal Campsites',
                description: 'This part contains information about seasonal campsite occupancy, membership, site coordinators, conditional members, seasonal campsite development, and more.',
                content: [
                    {
                        heading: 'Seasonal Campsite Occupancy',
                        body: '',
                        list: [
                            'All groups of members occupying a TRC seasonal campsite will appoint a Site Coordinator as a point of contact who is responsible to pass information/ concerns and collect fees on behalf of the campsite. ',
                            'Dates for the seasonal setup and closure of seasonal campsites shall be established by the Board of Directors.',
                            'At the end of the season all sites are to be left closed in a clean and orderly state. User fees must be paid prior to closing. ',
                            'A fee, established by the Board of Directors, will be charged to member(s) for the removal and storage of any abandoned items. Items not claimed within 30 days will become the property of TRC. ',
                        ]
                    },
                    {
                        heading: 'Membership',
                        body: 'All registered members of the campsite shall keep their TRC membership valid and continuous while claiming occupancy of a TRC seasonal campsite',
                    },
                    {
                        heading: 'Site Coordinators Responsibilities',
                        body: ' Site coordinators are the principal liaison between their site, its members, and TRC. The principal responsibilities of site coordinators are to:',
                        list: [
                            '▪ Maintain their site and coordinate the activities of the other members of their site.',
                            '▪ Inform Operations of who the members and/or conditional members of their site.',
                            '▪ Be the point of contact for resolution of any incidents involving the members of their site.',
                            '▪ Ensure adherence to all site occupancy, maintenance, and membership requirements.',
                        ]
                    },
                    {
                        heading: 'Site Coordinator Prerequisites',
                        body: '',
                        list: [
                            'No member of a seasonal site may be appointed coordinator unless they have been a member of said site for a minimum of 2 consecutive seasons. Exceptions to this rule require express approval by the VP of Ops (e.g. a site coordinator leaves a site and the remaining site members have only been with the site for 1 season). A regular member on the waiting list is exempt from this rule. ',
                            'Site coordinators must be on site for a minimum of two nights per month.',
                        ]
                    },
                    {
                        heading: 'Special Rules Regarding Seasonal Sites with a Single Member',
                        body: '',
                        list: [
                            'When a seasonal site’s membership consists of a single member who will be vacating their site at any time during the season, that member may not, under any circumstances, sell, trade, or add any new regular member as the site coordinator in order to ‘pass along’ the site to a person of their choice. ',
                            'The only exception will be if the transfer will be to the next member on the waiting list and approval is granted by the Seasonal Site Committee. ',
                            'Otherwise, the site will be considered ‘abandoned’ and the seasonal site will be granted to the next qualified member awaiting site placement.',
                        ]
                    },
                    {
                        heading: 'Conditional Members',
                        body: 'Conditional members are regular members who wish to join an existing seasonal site. The requirements to become a conditional member with a seasonal site are as follows:',
                        list: [
                            '▪ They must have been a regular member in good standing with fees paid in full for at least one season.',
                            '▪ The Site Coordinator for the seasonal site must inform the VP of Ops regarding the addition of a conditional member and have their name added to the sign-in sheet.',
                            '▪ One must be a Conditional member of a season campsite for one full calendar year before being recognized as an official seasonal member of the site.',
                            '▪ Once a conditional member has completed a full calendar year with a site, they may become a regular member of the site. This change must be reported to the SSC. A member cannot be a conditional member of the same site for more than two consecutive seasons. ',
                            '▪ Regular members cannot be involuntarily removed from the site without a unanimous vote of the other regular members, an action by the board, or a hearing before the SSC.',
                        ]
                    },
                    {
                        heading: 'Restrictions of Conditional Membership',
                        body: '',
                        list: [
                            'Conditional members may not bring guests to their site without a seasonal member of the site being present at TRC. Visitors are allowed for periods of less than six hours and not overnight for the purpose of socialization or site work but must have their own camp site.',
                            'A conditional member may not be selected as a site coordinator unless an exception is granted by the SSC and approved by the board. ',
                            'ALL exceptions to these rules must be approved by the SSC and the board.',
                        ]
                    },
                    {
                        heading: 'Seasonal Campsite Development',
                        body: '',
                        list: [
                            'No new campsites may be developed, land cleared, or tents pitched in undeveloped areas without the prior approval of the Development Committee.',
                            'No natural materials, native to the property should be moved or disturbed without prior approval of the Development Committee.',
                            'Seasonal campsites abutting property boundaries must be aware of those boundaries and must maintain a natural buffer between the properties and other campsites. ',
                            'Building of any new structure or platform of any kind without a permit from the Development Committee shall constitute the immediate suspension of membership of all those involved until further investigation by the Rules Committee. The Rules Committee will report their findings at the next Board of Directors meeting. Those found to be complacent in this infraction shall have their membership revoked and reviewed after a period of one year. ',
                            'Any site that has received a development permit from VP of Development, must post said permit in a conspicuous spot at the entrance to the site performing construction.',
                        ]
                    },
                    {
                        heading: 'Seasonal Site Occupancy',
                        body: 'No one may reside at TRC. At any time, the Executive Committee may request proof of residency.',
                    },
                    {
                        heading: 'Minimum Occupancy',
                        body: '',
                        list: [
                            'Seasonal campsites must be occupied by registered members who must sign in upon arrival and are actively camping for at least 4 nights in each calendar month. ',
                            'The site may not remain unoccupied for more than 19 consecutive days.',
                            'Failure to comply with the minimum occupancy rule and sign-in procedures may result in the loss of Seasonal camping privileges. ',
                            'Any exceptions to these requirements must be reviewed, approved, and documented by the VP of Operations. Decisions of the VP may be appealed to the board.',
                        ]
                    },
                    {
                        heading: 'Guests',
                        body: '',
                        list: [
                            'Members are responsible for the behavior and payment of camping fees for their guest(s).',
                            'Seasonal sites that have guests who do not pay their camping fees may be fined $20/night in addition to any unpaid camping fees.',
                            'No guest may be allowed on a seasonal site prior to the arrival or after the departure of a member of that site without prior verbal or written notification given to the VP of Operations.',
                        ]
                    },
                    {
                        heading: 'Guest Memberships',
                        body: '',
                        list: [
                            'A guest membership is a limited, non-voting membership which may be purchased by any regular member.',
                            'All guests must meet the membership requirements of TRC and register with the camp host upon arrival.',
                            'At registration, the guest must be accompanied by the Sponsoring member. ',
                        ]
                    },
                    {
                        heading: 'Enforcement of Occupancy Conditions (Sections 3-11)',
                        body: '',
                        list: [
                            'If a site has failed to meet the requirements of this section, the VP of Operations or their designee will notify the site coordinator and ask them to remedy the situation within 14 days.',
                            'If after the waiting period the site is still not in compliance or violates this section a second time during the same season, the VP of Operations or their designee will notify all registered campsite members and ask them to remedy the situation within 14 days.',
                            'If after the second waiting period, the site is still not in compliance or a third violation occurs during the same season, the VP of Operations will recommend to the Board of Directors to revoke the site membership of all registered members.',
                            'Site members may ask the Board of Directors SSC for a hardship exemption from the Minimum Occupancy obligations for up to a single season. ',
                        ]
                    },
                    {
                        heading: 'Enforcement of Membership Conditions (Section 2)',
                        body: '',
                        list: [
                            'Regular members of TRC will be notified by the treasurer when their membership is within 30 days of expiring.',
                            'If a seasonal campsite member’s membership with TRC has lapsed for more than 30 days, the member will be removed from the list of registered members for the campsite.',
                            'If the site coordinator is removed from a seasonal campsite, the remaining eligible site members are to nominate their own choice for coordinator. If the remaining eligible site members are unable to reach a decision by the next Board meeting, the Board of Directors will select the new coordinator from the remaining eligible site members.',
                            'If there are no eligible members registered for a site, the site will be considered abandoned.',
                            'Seasonal members that wish to camp with an expired membership must pay the limited camping fees of TRC. These fees may and will be credited towards membership dues if paid in full within 30 days.',
                        ]
                    },
                    {
                        heading: 'Notification',
                        body: 'Whenever it is necessary to notify a regular member of TRC, the person responsible to give notice must do all of the following:',
                        list: [
                            '▪ Send a copy of the notice via the United States Postal Service to the address provided on the member’s most recent application.',
                            '▪ Leave a copy of the notice at the member’s seasonal campsite.',
                            '▪ Send an email to the address provided on the member’s most recent application.',
                            'The person responsible for giving notice is encouraged to use any means which is likely to inform the member of the situation; however, the preceding requirements for notice must be met. ',
                        ]
                    },
                ],
                href: '#seasonal-camping-c',
                id: 'seasonal-camping-c',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Seasonal Site Maintenance & Upkeep Policy',
                description: 'This part contains information about seasonal site maintenance and upkeep, including fire safety, water usage, electrical, trees, and non-compliance.',
                content: [
                    {
                        heading: 'General Requirements',
                        body: '',
                        list: [
                            'All Seasonal Sites shall maintain a reasonably clean and tidy site free of obvious waste and visual abandonment.',
                            'Any designated sleeping area shall be maintained and setup during the regular open camping season period. Without this, the minimum occupancy rule cannot be in effect for the site.',
                            'There shall be a reasonable use or decorative function for items at the site. There shall be no collection of refuse or other items of obvious trash-like status. ',
                            'All sites shall be maintained so that they are usable and accessible.',
                            'Reasonable exceptions may be granted by either the VP of Operations or the VP of Development. These include, but are not limited to, construction, damage, health, etc.',
                        ]
                    },
                    {
                        heading: 'Fire Safety',
                        body: '',
                        list: [
                            'If a site has enclosed structures with electrical wiring or propane appliances, each of these structures must have an ABC type fire extinguisher inside.',
                            'Each site must have a minimum of two 5-gallon fire buckets filled with water on site at all times. One is to be kept at the main entrance and the other near the fire pit.',
                            'Any site with either a fire suppression water connection or water tank shall have a hose connected that is of sufficient length to reach all points in the site. This hose should be affixed to either a red 4x4 post or to a section of structure wall painted red.',
                            'The fire marshal will inspect all seasonal sites at least once per year to ensure compliance with the fire safety policy. Any violations need to be corrected within 14 days.',
                        ]
                    },
                    {
                        heading: 'Water Usage',
                        body: '',
                        list: [
                            'Seasonal sites may maintain a water tank for the purposes of fire suppression',
                            'Black water may not be dumped anywhere on TRC property and is to be disposed of in accordance with county and state laws.',
                            'Gray water is to be disposed of appropriately and never dumped within 50 feet of a stream or riverbank.',
                            'Any device used for the collection of water for decorative purposes larger than a common bird bath shall require approval from the VP of Development.',
                            'Pools, hot tubs, and the like, are prohibited',
                        ]
                    },
                    {
                        heading: 'Electrical',
                        body: '',
                        list: [
                            'Electrical wiring shall be installed in a manner to prevent accidental electrocution and fire. This includes using appropriately rated extension cords and UFB (Underground Feeder – Burial) wire were exposed to the elements or buried.',
                            'Each site may connect to the camp grid after paying the annual fee.',
                            'Each site is limited to a single 20A 120V connection to the grid. Sites hosting TRC events may use additional connections for the duration of the party. Such additional usage should be coordinated with the VP of Operations.',
                            'High wattage appliances such as electric heaters, microwaves, griddles, air conditioners and the like are not to be connected to the TRC grid at any time. Limited usage of power tools is acceptable, provided that such usage does not overtax the grid section.',
                            'Personal generators must not be audible to neighbors after 10 PM',
                        ]
                    },
                    {
                        heading: 'Trees',
                        body: '',
                        list: [
                            'Standing trees (dead or alive) are not to be felled without the approval of the Vice President of Development. Submit a maintenance request form to request evaluation of problem trees.',
                            'A rubber or wood buffer must be used when affixing cables, chains, or similar metal items to a tree.',
                            'Do not drive any nails, screws, or other fasteners into trees. These items can damage equipment or cause injury when felling trees.',
                            'Ensure that tarp lines and other items tied to trees are not causing damage. Action should be taken as soon as possible if any line is girdling or otherwise damaging the tree',
                        ]
                    },
                    {
                        heading: 'Non-Compliance',
                        body: '',
                        list: [
                            'If a site appears to be in noncompliance with the above rules, the VP of Operations or the VP of Development shall submit a report to the Site Coordinator, Seasonal Site Committee, and the VP of Member Relations.',
                            'The site coordinator shall have seven (7) days to respond with an action plan to rectify the situation. If the site coordinator does not agree that the site is out of compliance, an appeal may be filed with the Seasonal Site Committee.',
                            'The VP initiating the action and the VP of Member relations will work to approve the action plan within seven (7) days. ',
                            'Once the action plan is approved, the site members shall have thirty (30) days to show significant improvement in the condition of the site. After this period, the initiating VP and VP of Member Relations will reevaluate the situation to determine if further remedial action is necessary.',
                            'If, after thirty (30) days, no reasonable effort has been made to maintain the site, the site abandonment procedure shall begin.',
                            'Any situation that places the life or health of a member at risk, such as bare wires, severely deficient structures, and the like may require more immediate remediation.',
                        ]
                    },
                ],
                href: '#seasonal-camping-d',
                id: 'seasonal-camping-d',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Alcohol Service',
                description: 'All individuals are held to responsible alcohol service and consumption at their sites.',
                content: [
                    {
                        heading: 'Responsible Alcohol Service',
                        body: '',
                        list: [
                            'Site members are responsible for responsible alcohol service at their sites.',
                            'Alcohol is not to be provided to any person who is already intoxicated. Service of alcohol to an already intoxicated person shall be considered a violation of camp rules, even if no other infraction occurs as a result.',
                            'Overservice of alcohol by a site will be considered a complicit act to any rule violations by the guest or visitor who was overserved. If any guest served by a site member(s) commits a rules violation, determined to be principally due to over-intoxication, said site member(s) may be considered complicit in the infraction.)',
                            'Sites with repeated violations of the policy may have camping privileges suspended for those site members in violation.',
                        ]
                    },
                ],
                href: '#seasonal-camping-e',
                id: 'seasonal-camping-e',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Overwinter Storage Policy',
                description: 'This part describes the overwinter storage policy and for seasonal sites.',
                content: [
                    {
                        heading: 'Required Actions',
                        body: '',
                        list: [
                            'By October 15th (no exceptions) of a given camping season, all seasonal sites shall be disassembled to a reasonable level of security for the winter months.',
                            'Sites are required to stay disassembled in this matter until the “Soft Opening” date announced by the VP of Operations. ',
                            'This includes the following: tarps, unsecured items and property, camping gear (tents, etc.), eating areas, water suppression system, water storage systems, and any other property capable of causing damage to neighboring sites or TRC property over the winter months.',
                            'The VP of Operations or their designee(s) shall do periodic walk-throughs in the month of October to ensure sites are securely broken down. ',
                            'If the members of a site have a question as to the sufficiency of their winterizing procedures, it is their responsibility to inquire upon the VP of Operations for clarification and/or approval of a given procedure.',
                        ]
                    },
                    {
                        heading: 'Non-Compliance',
                        body: '',
                        list: [
                            'Any site not in compliance with this policy (aka “Winter Teardown”) shall be considered abandoned and subject to the TRC Abandonment Policy, unless PRIOR arrangements have been made with the VP of Operations.',
                            'TRC shall be reimbursed for any and all costs incurred in order to secure a seasonal site in the winter months. Any amounts owed to TRC shall be divided equally among the members currently registered with the site. Those members shall not camp at TRC until their portion of the debt has been paid.',
                        ]
                    },
                ],
                href: '#seasonal-camping-f',
                id: 'seasonal-camping-f',
                imageUrl:
                    camping_1,
            },
            {
                title: 'TRC Abandonment Procedure',
                description: 'This part describes the TRC abandonment procedure for seasonal sites.',
                content: [
                    {
                        heading: 'Determination of Abandonment',
                        body: 'Once a site has been deemed abandoned by the VP of Operations, either by:',
                        list: [
                            '▪ Notification by the current site members of intent to abandon.',
                            '▪ Site Maintenance Policy violations.',
                            '▪ Other conditions under which a site may have no members.',
                        ]
                    },
                    {
                        heading: 'Abandonment Procedure',
                        body: '',
                        list: [
                            'A “Letter of Abandonment” shall be sent via email to all site members.',
                            'Site members have 72 hours from the date of the email to respond to the VP of Operations with an action plan of claiming their belongings.',
                            'Once the VP of Operations approves the action plan, exiting site members shall remove their personal belongings and refuse from the site on the date(s) and time(s) agreed upon in said action plan. The VP of Operations, in their sole discretion, may extend the time permitted for this removal and clean-up process. However, under no circumstances shall the allotted time exceed thirty (30) days.',
                            'If there is no response from any site member within seventy-two (72) hours of receipt of the dated Letter of Abandonment, the site shall be considered abandoned and all items left on the site become property of TRC. ',
                            'TRC shall be reimbursed for any and all costs incurred relating to the abandonment. Any amounts owed to TRC shall be divided equally among the site members currently registered with the abandoned site. Those members may not camp at TRC until their portion of the debt has been paid.',
                        ]
                    },
                ],
                href: '#seasonal-camping-g',
                id: 'seasonal-camping-g',
                imageUrl:
                    camping_1,
            },
        ]
    },
    {
        title: 'Section Title',
        description: 'This section contains the',
        id: 'sectionid',
        parts: [
            {
                title: 'Part A Title',
                description: 'This part describes',
                content: [
                    {
                        heading: 'Item Heading',
                        body: '',
                        list: [
                            '',
                            '',
                        ]
                    },
                ],
                href: '#part-a',
                id: 'part-a',
                imageUrl:
                    camping_1,
            },
            {
                title: 'Part B Title',
                description: 'This part describes',
                content: [
                    {
                        heading: 'Item Heading',
                        body: '',
                        list: [
                            '',
                            '',
                            '',
                        ]
                    },
                    {
                        heading: 'Item Heading',
                        body: '',
                        list: [
                            '',
                            '',
                            '',
                            '',
                        ]
                    },
                ],
                href: '#part-b',
                id: 'part-b',
                imageUrl:
                    camping_1,
            },
        ]
    },
]
</script>