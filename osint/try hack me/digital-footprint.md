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
# 2.archived company website
> ACME Jet Solutions (warc-acme.com/jef/), is all over social meda claiming they were founded in 2025 and that they're the fastest-growing data company in Africa.
> But something doesn't add up, one of their ex-employees ensures you that the company existed long before that. Your job as an OSINT investigator is to verify their founding date using only public information.
>
> When was the website first published on the internet?
## walkthrough
mình vào [wayback machine](https://web.archive.org/web/20260000000000*/warc-acme.com) để xem lịch sử trang, tuy nhiên không có kết quả

<img width="1258" height="608" alt="Screenshot 2026-09-17 172329" src="https://github.com/user-attachments/assets/d98732d7-2496-4f88-bb4f-9dd252c8026c" />

sau đó mình tìm hiểu thì biết wayback machine calendar chỉ hiển thị các trang đã được hệ thống xử lý và index chính thức. nếu ai đó upload thẳng tệp .warc thô lên internet archive như một item độc lập thì nó sẽ không xuất hiện ở đó, vì vậy mình chuyển sang search

<img width="1259" height="658" alt="Screenshot 2026-09-17 191501" src="https://github.com/user-attachments/assets/a97a1527-18ad-4d56-9706-c5292caa58fa" />

lúc này đã tìm thấy thời điểm đầu tiên web được đăng lên internet

<img width="1239" height="688" alt="Screenshot 2026-09-17 191537" src="https://github.com/user-attachments/assets/24f5df7e-45ce-4feb-9a89-fbe4fd29b12f" />

-> Firstfiledate: 20160210224602
## flag
`THM{20160210224602}`
---
# 3.mysterious landmark
> Further Investigation uncovers another image believed to be connected to the company's international expansion. Research reveals that to the right of the iconic landmark is a building that played a big role in the fight for independence of a particular country. Signs on the external wall provides the name of the building. Submit the name of building translated into English as the flag.
> 
> <img width="3456" height="4608" alt="landmark-1763035881792" src="https://github.com/user-attachments/assets/1636d43b-26f5-40f2-881c-ebcd2f65f35d" />
>
> What is the landmark?
## walkthrough
mình tra địa điểm của bức ảnh qua google search ảnh 

<img width="1250" height="692" alt="Screenshot 2026-09-18 142701" src="https://github.com/user-attachments/assets/1e2118bd-bf48-4a4b-9086-d937a19093a1" />

kiến trúc trong bức ảnh là the spire ở ireland, sau đó mình vào map để tìm địa điểm của kiến trúc trên

<img width="1262" height="689" alt="Screenshot 2026-09-18 142930" src="https://github.com/user-attachments/assets/5e7de6ba-e8c5-4019-927e-440ea179f00c" />

phía bên phải của kiến trúc trên là general post office 
## flag
`THM{General Post Office}`
---
# 4.internal documents
> After uncovering ACME Jet Solutions origins and tracing their online presence through archived websites and international landmarks, investigators believe that an internal document was accidentally leaked by one of the company's developers.The document may contain crucial information about the individual responsible for maintaining their systems. 
>
>[internal-docs-1769695301727.odt](https://github.com/user-attachments/files/32370654/internal-docs-1769695301727.odt)
>
> What is the final flag?
## walkthrough
sau khi tải file .odt về, mình đổi thành file .zip và giải nén ra

<img width="456" height="261" alt="Screenshot 2026-09-18 145444" src="https://github.com/user-attachments/assets/d5870892-4e43-4734-9273-7fab1ba83108" />

mình quét từng file một và khi quét đến meta.xml, mình phát hiện được username của mark là "markwilliams7243"

<img width="975" height="260" alt="Screenshot 2026-09-18 145708" src="https://github.com/user-attachments/assets/1927936c-d62c-400a-971a-a2c5b23b253c" />

sau đó mình tìm kiếm username trên web, và nó xuất hiện 1 kênh [youtube](https://www.youtube.com/@markwilliams7243) của mark

<img width="1073" height="703" alt="Screenshot 2026-09-18 145841" src="https://github.com/user-attachments/assets/195c8670-534e-4f0d-98fb-fa69fbe7b0e5" />

và đã tìm được flag
## flag
`THM{Y0u_f0und_7h3_fin4l_fl4g!}`






