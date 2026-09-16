# overview
- nền tảng: [try hack me](https://tryhackme.com)
- room: [digital footprint](https://tryhackme.com/room/osintchallengeiv)
- catergory: osint
---
# 1.the leaked photo
> An ACME Jet Solutions employee uploaded a photo of a residential property believed to be linked to ACME Jet's early operations. Can you figure out where the picture was taken to confirm or debunk the rumour?
>
> <img width="1306" height="837" alt="edited-house-1763031553617" src="https://github.com/user-attachments/assets/d58fd1d8-9d9f-40fa-ac62-e372892105ea" />
>
> In which city was the photo taken?
## walkthrough
mình dùng exif tool để tìm gps longtitude và latitude của ảnh trên

<img width="540" height="341" alt="Screenshot 2026-09-17 043348" src="https://github.com/user-attachments/assets/f773b37b-5164-4e8d-8368-ee859357f298" />

rồi mình vào [gps coordinates](https://www.gps-coordinates.net/) copy paste tọa độ vừa nãy rồi search địa điểm, lúc này có 4 options: north, south, east, west mình thử từng cái và thấy south east là phương án hợp lý nhất

<img width="1253" height="692" alt="Screenshot 2026-09-17 044120" src="https://github.com/user-attachments/assets/cfdfca90-fa2f-4466-adba-16226f6a3162" />

-> địa điểm là ở johannesburg, south africa
## flag
`THM{Johannesburg}`
---
# 2. archived company website
> ACME Jet Solutions (warc-acme.com/jef/), is all over social meda claiming they were founded in 2025 and that they're the fastest-growing data company in Africa.
> But something doesn't add up, one of their ex-employees ensures you that the company existed long before that. Your job as an OSINT investigator is to verify their founding date using only public information.
>
> When was the website first published on the internet?




