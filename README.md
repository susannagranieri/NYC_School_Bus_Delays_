By Mariana Castro & Susanna Granieri, **May 2022**

After over a year of remote learning, New York City school buses were back on the road for the 2020-2021 school year, but, complaints of late buses, or even no-shows, occur often. Data surrounding these delays, including delay times, vendors, school addresses and boroughs, paint an assumed, but question-provoking picture.

We decided to look into New York City's school bus delay data. This dataset, found on NYC Open Data, was last updated on Nov. 24, 2021. It includes all bus delays between January and June 2021, as well as the length of those delays, the reason, the Office of Pupil Transportation (OPT) information, the route identifier, the run type (AM or PM) and the date the delay occured. The OPT code information provides the school name, their addresses, phone numbers, district, borough and school type.

Using Python, we combined the bus delay data from Open Data and the OPT code information to match the name and addresses of the schools in which a delay was reported.

We were curious as to how many buses were delayed due to mechanical issues, so we filtered our data to find that information.

We then filtered our data again to find how many each vendor reported. Is there any particular company that is responsible for the most bus delays attributed to mechanical problems?

                    BORO TRANSIT, INC.                     542
                    RELIANT TRANSPORTATION, INC (B2321)    222
                    SNT BUS INC                            221
                    PRIDE TRANSPORTATION (SCH AGE)         203
                    HOYT TRANSPORTATION CORP.              200
                    QUALITY TRANSPORTATION CORP.           197
                    LITTLE RICHIE BUS SERVICE              181
                    PIONEER TRANSPORTATION CORP            158
                    JOFAZ TRANSPORTATION INC.              125
                    LORINDA ENTERPRISES, LTD.              114
                    LEESEL TRANSPORTATION CORP (B2192)     107
                    Y & M TRANSIT CORP (B2192)              88
                    GRANDPA`S BUS CO., INC.                 76
                    BOBBY`S BUS CO. INC.                    71
                    L & M BUS CORP (A)                      59
                    CONSOLIDATED BUS TRANSIT, INC.          54
                    LOGAN BUS COMPANY INC.                  53
                    ALLIED TRANSIT CORP.                    42
                    FIRST STEPS TRANS INC. (B2192)          39
                    G.V.C., LTD.                            35
                    LORISSA BUS SERVICE INC.                29
                    B & F SKILLED INC.(B2192)               29
                    DON THOMAS BUSES, INC.                  25
                    VAN TRANS LLC (B2192)                   24
                    DON THOMAS BUSES, INC. (B2321)          22
                    THOMAS BUSES, INC. (B2321)              22
                    EMPIRE CHARTER SERVICE INC              21
                    L & M BUS CORP.                         17
                    LITTLE LISA BUS CO. INC.                16
                    EMPIRE STATE BUS CORP.                  14
                    ALL AMERICAN SCHOOL BUS CORP.           13
                    PHILLIP BUS CORP (B2192)                13
                    G.V.C. LTD. (B2192)                     12
                    PHILLIPS BUS SERVICE                    10
                    LOGAN TRANSPORTATION SYSTEMS             9
                    FIRST STEPS TRANS, INC                   9
                    THOMAS BUSES INC (B2192)                 7
                    I & Y TRANSIT CORP                       6
                    MAR-CAN TRANSPORT CO. INC (B2192)        4
                    THIRD AVENUE TRANSIT, INC                3
                    ALINA SERVICES CORP.                     3
                    SELBY TRANSPORTATION                     3
                    CHILDREN`S TRANS INC. (B2321)            3
                    CAREFUL BUS SERVICE INC (B2192)          2
                    CAREFUL BUS                              2
                    ANOTHER RIDE INC.                        2
                    MONTAUK STUDENT TRANS LLC (B2192)        1
                    VINNY`S BUS SERVICES (B2321)             1

But, were mechanical problems the top reason for bus delays?

                    Heavy Traffic: 18,143
                    Other: 4,078
                    Mechanical Problem: 3,109
                    Won`t Start: 770
                    Flat Tire: 714

No. "Heavy traffic" actually landed at number one, which we assume is due to New York City congestion. "Other" came in second, which is not described in the data dictionary. So we focused on the third.


We looked into the top five companies on the list above: Boro Transit, Inc., SNT Bus Inc., Pride Transportation, Quality Transportation Corp. and Reliant Transportation, Inc.
We found that Boro Transit, Inc. and SNT Bus Inc. are located at the same address (50 Snediker Avenue, Brooklyn, NY 11207), have the same phone number (718-346-9600) and email address (consolidatedbus@cbttrans.com). In further investigation, we found that Jodi Curcio-Genovese is the owner of the two companies.

It seems as though the companies consolidated to become Consolidated Bus Transit Inc. When you Google SNT Bus Inc., the address for Consolidated Bus Transit is also a result. But the address is 38 Snediker on Google, but on their website it is 68 Snediker — not 50 Snediker like Boro Transit, Inc.

Boro Transit, Inc., after searching for it on Google, shows a 1.6/5 star rating based on nine reviews. Most, if not all, were not complimentary of the company.
  “My daughter has special needs and goes to a private school, we were told by the bus coordinator at the school no masks were required on the bus as she falls under the exceptions outlined by OPT,” wrote reviewer Joe R M last year. “First day of school, she came home with a mask around her neck, red marks behind her head and ears ,smelling of latex around her face and hair, and in complete distress because apparently she was FORCED into the mask by the matron and or driver! That's assault.”

Their lateness is assumed due to the 542 delays caused by mechanical problems.
  “[Their] service sucks. I was waiting for 2 hours for my son to be [picked] up at 6:30 a.m. and they never arrived. No one called me to tell me anything, nor the bus driving or the company,” another reviewer wrote. “I called them thousands of times and their phone was always busy and I finally got through and the woman [who picked up] was rude and didn’t care, she said anything to get me off the phone. So I made a report on them. [Their] service sucks.”


**Quality Transportation Corp.**

New York City, according to the New York Post, granted a pay increase to Quality Transportation Corp. Their contract was extended, and their pay "rose from an original 
270.3 million for nine years through June 2023." The safety of these companies had not been checked, nor the experiences reported by loved ones and students. Last year, 10-year-old Patience Albert was struck and killed by Pedro Colin, 61, after he turned at a four-way intersection and Albert was crossing the street — there were stop signs on all four streets.

Back in September, the issues with NYC's bus companies, although living with a bad track-record, were a real-time, live issue. After the pandemic shut down New York City schools for over a year, many students were excited for their first day back — but their school buses never showed. Chalkbeat reported that, at the time, almost 1 million students were going to school for the first time since the pandemic, but parents reported delays and complained to OPT. At the time of the article, though, there was no data backing up this experience because school's had been closed for so long. Now, with the new bus delay data, the extent of the issues can actually be quantified and analyzed.

We also decided to geocode the data to find what neighborhoods in New York City dealt with the most school bus delays from this particular time frame as a result of a reported "mechanical problem." 

In this heatmap, you can see the areas that are impacted by delays caused by mechanical problem.

<img width="837" height="753" alt="Screenshot 2025-07-16 at 12 56 59 PM" src="https://github.com/user-attachments/assets/92c14ff2-7926-4747-b151-362169c4e7e1" />

If we were to overlay the neighborhoods of Brooklyn, the highest intensity would land in the Bay Ridge, Borough Park, Sunset Park, Prospect Park or Bensonhurst areas.

