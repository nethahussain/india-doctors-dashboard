# Post text for the six slides

Images: `png/slide-1.png` … `png/slide-6.png`, 1080 × 1350 (4:5), in that order as one carousel / multi-photo post.
To change a slide, edit `slides.html` and re-render (see the end of this file).

## Instagram caption

Where do India's 1.7 million registered doctors live, and who are the new ones? 🩺

I downloaded every record on the national medical register (NMC Indian Medical Register) and turned it into charts:

📍 Doctors cluster in the south and around the big cities
👩‍⚕️ In Andhra Pradesh, Telangana and Kerala, women have outnumbered men among new doctors every year since the mid-2010s
📊 Sikkim and Karnataka have over 25 registered doctors per 10,000 people; Bihar and Jharkhand under 3
🌍 About 99,000 registered doctors studied abroad, half of them in China, Russia or Ukraine
📈 87,500 doctors joined the register in 2025, almost six times as many as in 1990

Explore your own state: link in bio 👉 nethahussain.github.io/india-doctors-dashboard

Notes: gender is estimated from first names; the register counts where doctors registered, not where they work; only aggregate counts are published.

#India #Doctors #MedicalEducation #WomenInMedicine #DataVisualization #DataViz #PublicHealth #HealthWorkforce #NMC #OpenData #Kerala #Karnataka #TamilNadu #Telangana #AndhraPradesh

## Facebook post

How many doctors does India have, where do they live, and who are the new ones?

I downloaded all 1.73 million registrations on India's national medical register (NMC Indian Medical Register, November 2026) and built an interactive dashboard where you can pick any state. A few things that stood out:

• Doctors are far from evenly spread. Sikkim (34) and Karnataka (28) have the most registered doctors under 65 per 10,000 people; Bihar and Jharkhand have fewer than 3. India as a whole: about 11.
• In Andhra Pradesh, Telangana and Kerala, women have outnumbered men among newly registered doctors every year since the mid-2010s.
• About 99,000 registered doctors earned their medical degree abroad. China, Russia and Ukraine trained almost half of them.
• 87,500 doctors joined the register in 2025, almost six times as many as in 1990, and that's an undercount, because several state councils have stopped sending new entries to the national register.

Explore the numbers for your state: https://nethahussain.github.io/india-doctors-dashboard/

A few caveats: the register has no gender field, so gender is estimated from first names; it shows where doctors registered, not where they work; and doctors registered in two states are counted twice (about 2.4% of records). Only aggregate counts are published.

## Alt text (one per slide)

1. Map of India with blue dots for PIN code areas, sized by how many registered doctors live there. The dots are densest in Kerala, Tamil Nadu and Karnataka, and around Delhi, Mumbai, Kolkata and Hyderabad.
2. Line chart of women's share of new doctor registrations, 2000 to 2025, for Andhra Pradesh, Telangana and Kerala. All three rise from about 40% to above 50% around 2015. The latest values are Telangana 57%, Andhra Pradesh 53% and Kerala 56% (2019).
3. Bar chart of registered doctors under 65 per 10,000 people in 2026. Highest: Sikkim 34.2, Karnataka 27.9, Goa 27.7, Tamil Nadu 23.1, Kerala 22.9. India 10.8. Lowest: Chhattisgarh 5.8, Madhya Pradesh 5.5, Uttar Pradesh 4.3, Bihar 2.8, Jharkhand 2.8.
4. Bar chart of countries where foreign-trained doctors got their degree: China 20,215, Russia 16,924, Ukraine 11,434, Nepal 10,149, Philippines 7,719, Kyrgyzstan 5,913, Bangladesh 5,457, Kazakhstan 4,462, Armenia 1,999.
5. Column chart of new registrations per year from 1960 to 2025, rising slowly to 15,133 in 1990 and steeply after 2005 to 87,519 in 2025.
6. Summary card: 1.69 million distinct doctors, 1.40 million under 65, 10.8 doctors under 65 per 10,000 people, 30 medical councils. Link: nethahussain.github.io/india-doctors-dashboard. Created by Netha Hussain.

## Re-rendering

From the project folder, serve it and screenshot each slide with Chrome:

```bash
python3 -m http.server 8768
```

```bash
for s in 1 2 3 4 5 6; do "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --hide-scrollbars --force-device-scale-factor=1 --window-size=1080,1350 --virtual-time-budget=15000 --screenshot="social/png/slide-$s.png" "http://localhost:8768/social/slides.html?s=$s"; done
```
