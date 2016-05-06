---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
keywords: []
description: 'As a traveling physicist I have the opportunity to work with a variety of equipment that has been purchased for various reasons by other physicists over the years. There’s really two technology choices that impact the daily life of a physicist and both are expensive enough that we rarely get to make them in our career and even more rarely will have had experience with the different choices in anything other than a demonstration by the vendor. So to help with optimizing these choices I thought I’d publish my opinion, which I’ll state is only one physicist’s opinion, and no, I do not have a financial interest in this besides helping others get the best bang for the buck.'
datePublished: '2016-05-06T14:54:25.392Z'
dateModified: '2016-05-06T14:53:59.624Z'
authors: []
publisher:
  name: null
  domain: null
  url: null
  favicon: null
title: ''
author: []
starred: false
sourcePath: _posts/2016-05-06-as-a-traveling-physicist-i-have-the-opportunity-to-work-with.md
url: as-a-traveling-physicist-i-have-the-opportunity-to-work-with/index.html
_type: Article

---
As a traveling physicist I have the opportunity to work with a variety of equipment that has been purchased for various reasons by other physicists over the years. There's really two technology choices that impact the daily life of a physicist and both are expensive enough that we rarely get to make them in our career and even more rarely will have had experience with the different choices in anything other than a demonstration by the vendor. So to help with optimizing these choices I thought I'd publish my opinion, which I'll state is only one physicist's opinion, and no, I do not have a financial interest in this besides helping others get the best bang for the buck.

The two technology choices I speak of are the choice of treatment planning system and the choice of device for IMRT QA. On the first, it appears to me to be a matter of faith, either you believe in Pinnacle or Varian, and there isn't much I can say to sway you either way. So I'll keep my remarks brief, Pinnacle is really antiquated and is inferior in all respects. If you liked Pinnacle, and/or have Elekta equipment, please move on to a modern TPS in Ray Station, you'll be doing your patients a favor. If you have Varian equipment, I can't think of a reason to venture beyond the Aria environment. Life is easy in a one vendor environment with one database.

But the second choice I will venture more boldly with a real review of IMRT QA equipment and I feel there is more to be gained by such. The following is a list of the equipment I have direct experience with in a clinical setting and my opinion of each.

* Mobius 3D
* Mapcheck
* ArcCheck
* Varian Portal Dosimetry
* IBA's MatriXX

Mobius is a new entrant and while I'd seen them at meetings I hadn't paid them any mind until a client had it. It is marvelous. I would compare this to experiencing indoor plumbing for the first time when you've only known an outhouse your entire life, and you lived in Grand Island, NE where the winters are frozen and summers are sweltering. Mobius works by utilizing the Dynalog files of leaf motion while simulating actual treatment with the actual fields. There's no second degree of separation with an IMRT QA plan, no setup to screw up, no gantry angle overrides, meaning gravity is effecting the leaves just as it will in treatment. And since there's no special setup required, it seems perfectly logical to me to have therapist run the QA on the machine at any point in the day when they have time. The Dynalog files are then uploaded to Mobius' web app which analyzes the motion vs. expected and then projects that back onto the CT and provides the physicist with a DVH to compare. Marvelous. There is no pondering what one pixel being 7% out means to the patient. There is no pondering if that 7% error is a calibration issue of that pixel. There is no pondering if your device setup was rotated, or translated. There's no pondering if it is in a dose gradient. It provides you with the data that you are actually interested in. Will this plan be delivered as planned and if not, what is the exact impact to the patient. This thing works perfect for both IMRT QA and VMAT QA. My conclusion, if you haven't looked at Mobius yet, ask them for a demo asap. Your mental ass will thank you for coming out of the cold.

MapCheck is the gold standard, with MapCheck 2 being the gold standard of the gold standard. If you're purchasing an IMRT QA device and you don't want to be criticized for your selection , go with the MapCheck 2\. MapCheck's diodes work well and with proper calibration (which is very easy, just follow the on-screen instructions) will give you excellent results with absolute dose with either Gamma or Dose, and Distance to Agreement. 3% and 3mm seems pretty standard on this, although I've seen 5% and 5mm used. I have seen this provide useful data with a string of plans failing for a bit being traced down to a dosimetrist using Eclipse and pushing the penalty into the range of \>400 which was causing leaf motion to exceed the machines ability to deliver. But honestly, I haven't any idea if this would of materially impacted the patient at all.

ArcCheck is a device I love as it works well and it is a 'cool' physics tool. But I can't recommend the ArcCheck at this point. While the ArcCheck was still in development Sun Nuclear put out a "MapPhan" which you slid the MapCheck into. And that worked, with errors in readings around 15 degrees around the sides of the device. But VMAT plans still passed just fine. I've been to plenty of sites using MapChecks with only their standard slabs of solid above and the VMAT QA comes out perfectly fine. At one point I thought to replace the MapCheck with the ArcCheck as this would allow me to do QA at the angle of treatment, but this doesn't work well in current versions of ArcCheck with the threshold activating bands of diodes instead of individual diodes, so your % difference at very small doses is wonk. Conclusion, save your money, use your MapCheck 2 for your VMAT QA, it works just fine.

Varian Portal Dosimetry is a concept that at first blush appears brilliant. Simple, comes with the machine, easy setup, and there is where it all goes wrong. I've used Portal Dose at several centers and never once does it actually work well. I mean, it works, but not well. You end up with pixels or more likely patches of pixels that are wonk, they just don't work. Often times you'll have borderline to failing QA's which when measured by different equipment are just fine. This is wholly an unsatisfactory state of affairs. Speaking with Varian helps one gain an understanding of the equipment and its failures, but it doesn't leave you with the warm fuzzies of feeling like your IMRT plan is safe. Unless Varian is going to throw this in for free (which they sometimes do) on a new install AND you have an extremely frugal administration, look elsewhere for your QA needs. Of important note is that Mobius uses the same equipment and the experience is radically different...hint, hint, Varian, your issue lies in the software vs. the hardware.

And then there is the also ran of IMRT QA devices. The IBA MatriXX device. This device is absolutely the worst of the lot. After a two hour conversation with "the" IBA Matrix engineer I concluded by stating to him "it is unethical for you to keep this device on the market." It's awful. Difficult setup (especially if you try to do the gantry mount), inability to do anything other than relative dose, poor operation, and if you're especially masochistic try using the Compass utility. I cannot express how awful this experience was, and all the while knowing it was 2x the expense of a Matrix 2, oh my god, I pity the physicist that ends up with this device. Conclusion, avoid at all costs and IBA please take this product off the market as it is worst in class.