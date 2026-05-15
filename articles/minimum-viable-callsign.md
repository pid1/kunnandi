## Minimum Viable Callsign

I got my amateur radio technician license last month. On the air for under $200, I studied on paternity leave, and the whole setup is a minimum viable callsign: cheap enough to throw away, complete enough to operate, deliberately built for replacement.

I am KJ5PTV today, KA1PID once the FCC processes my vanity request. pid1, on the air.

### What I wanted

#### Emergency Communications

Most of the emergency theater I have seen in IT involves operational procedures that have never been tested. I refuse to bring that mindset into a hobby. I wanted a station I could use if cell, power, and Internet were out, not a station I theorized would work in an emergency. By using my emergency station as my daily driver, I know it will work when I need it to.

#### A hobby, not more work

I have been a technologist for decades. Internet-bridged systems like EchoLink, AllStarLink, IRLP, and Wires-X solve a different problem than the one I am solving, and they are adjacent to everything I already do. If I wanted to talk to people across a network, I have Discord, Slack, VoIP, Zoom, and a dozen other tools. The whole point of radio is the radio.

#### Simplicity

Analog FM is the lingua franca on 2m and 70cm. Anyone with a VHF or UHF radio in range can hear me. Digital modulation like DMR, D-STAR, YSF, or M17 splits the on-air community across incompatible codecs. They are technically interesting, and I will probably get there eventually. For year one, the goal is to show up on the local repeater and be heard by everyone, not by a subset of people who bought the same brand of radio I did.

Pure FM, locally repeated or simplex, no internet involved.

### Studying on paternity leave

With a three-year-old, a one-month-old, and a demanding career, there are no quiet evenings.

The paternity leave I took doubled as my study window. I studied two ways. HamStudy.org on my phone, in five and ten-minute fragments between feedings and naps, ensured I was ready for the test environment. Ham Radio Crash Course on YouTube has videos on the technician question pool. Playing these at 1.5x while I walked the baby and folded laundry made that time productive.

The audio format is what made it work. Test when HamStudy says you are passing at 85% consistently.

### The real Technician exam

The Technician exam is 35 multiple-choice questions. The FCC website is the actual exam.

To get a callsign, you need an FRN. To get an FRN, you log into CORES. To pay your $35, you log into a different portal. To file your vanity request, you log in to ULS, which is technically the same system but does not feel like it. Each surface has its own session, its own UI from 1998, and its own login flow that may or may not now route through login.gov depending on which page caught you.

### The hardware

The starting station is deliberately cheap and deliberately uninteresting.

- Baofeng UV-5RM Plus, around $25. A dual-band handheld, 8W, USB-C charging. The transmitter is rough by professional standards, the firmware is utilitarian, and the build is plastic. None of that matters for the job it is doing right now.
- Nagoya NA-771, around $20. A 15.6-inch dual-band whip that replaces the stock rubber duck on the Baofeng.
- Magnetic dual-band antenna for my car, around $20. The Baofeng with any HT whip inside a metal vehicle is barely a radio. With the antenna on the roof, it becomes usable.
- RTL-SDR at home, running rtl_tcp. About $60 with antenna kit. Accessible over Tailscale, which is free.
- CoronaSDR on the phone. Free. Silviu YO6SAY's iOS client for rtl_tcp servers, released earlier this year.

CoronaSDR makes the setup shine. I transmit from the Baofeng in the field, listen to 146.92 on my phone via the home SDR, accessible over Tailscale, and verify the repeater is coming back clean, even if nobody is on it to respond. Self-contained, no human in the loop, repeatable. Exactly the kind of dark-tested infrastructure I would expect from any other system I depend on.

Total spend, including FCC and test fee, was well under $200. The point is not the rig. You can be licensed, on the air, and operating without spending thousands on hardware.

The Baofeng is a learning tool, not a duty rig. I can and probably will upgrade to something from Icom/Yaesu later, but this got me on the air without breaking the bank.

The Baofeng menu is hostile. CHIRP for programming is essential.

The hobby's deepest cultural problem is confusing gear acquisition with operating. I have no opinion on what radio you should buy. I strongly believe that you should be on the air with whatever you have or can afford.

### What's next

The General license opens HF, which is the actual answer to "communications that work without anyone else's infrastructure." NVIS on 40m or 80m off a wire antenna gets me regional coverage with nothing between me and the ionosphere. That is the version of the emergency-ready station I actually want, and the Technician privileges I have now are the apprenticeship for it.

Amateur Extra after that, mostly for completeness and for VE testing privileges.

GMRS as well. $35, no test, 10-year license, covers my whole immediate family on a single callsign, up to 50W mobile, repeater-capable. It is not a replacement for ham. It is the answer to "my wife and kids should be able to use the radios without studying for an exam." Different service, different use case, both worth having.

The training I am most interested in is Skywarn. North Texas Skywarn classes run early in the year, ahead of severe weather season. That is the first formal training on my list. It was disappointing to have to wait almost an entire calendar year before starting to participate.

MARS and ARES are further out. Both are real-time commitments, and time is the binding constraint right now. Two kids and a career leave little slack for monthly nets and quarterly drills. I will get there. I am not going to pretend I am there before I am.

If you are in North Texas, find me on The Mighty 92 or 146.52.

73,

KJ5PTV
