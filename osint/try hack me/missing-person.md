# overview
- platform: [try hack me](https://tryhackme.com)
- room: [missing person](https://tryhackme.com/room/missingperson)
- category: osint
---
# task 1: osint
> "My friend went on holiday in 2025 and shared some photos, but I haven’t heard from him since. Can you help me track him down for the police report?"
> 
> <img width="1360" height="765" alt="food" src="https://github.com/user-attachments/assets/0f5de9c8-9361-4720-bd19-fe01d13d5e1f" />
>
> <img width="960" height="540" alt="MotoGP" src="https://github.com/user-attachments/assets/6f3a1353-40de-427c-9228-4f1a33cf7b22" />
>
---
## 1.
> What is the commercial name of this circuit?
### walkthrough
mình tra ảnh trên trong google photo và tìm thấy tên của giải đấu

<img width="1243" height="689" alt="Screenshot 2026-09-19 22231" src="https://github.com/user-attachments/assets/ad89bb9d-0137-4408-a358-0aa2ab647ef0" />

## flag
`Pertamina Mandalika International Street Circuit`
---
## 2.
> When did the event take place?
### walkthrough
mình search thông tin của sự kiện trên ở google, sự kiện được tổ chức từ ngày 3 đến 5 tháng 10 năm 2025

<img width="1252" height="719" alt="Screenshot 2026-09-19 223446" src="https://github.com/user-attachments/assets/6d9b5cb1-0ce0-432f-b2a8-792a61d4feee" />

## flag
`03-05/10/2025`
---
## 3.
> He told me he ate delicious Mexican food. What is the name of the restaurant?
### walkthrough
lần này, mình dùng google search ảnh tiếp 

<img width="1217" height="686" alt="Screenshot 2026-09-19 png" src="https://github.com/user-attachments/assets/40ebea60-0128-4227-92f8-9b79a1536125" />

## flag
`Cantina Mexicana`
---
## 4.
> At what time was this photo taken?
### walkthrough
mình sẽ dùng exiftool để tìm thời gian ảnh được chụp lần đầu

<img width="737" height="419" alt="Screenshot 2026-09-19 230304" src="https://github.com/user-attachments/assets/50ca1e1b-4a95-4940-944a-d5dc45f7eb56" />

## flag
`19:55:30 `
---
## 5.
> He sent me a message, this is the last I heard from him: ”Went to this cool MotoGP after party, and became friends with one of the local DJs who played that night. We’re going to visit a cave tomorrow.”
> What is the full address of the bar’s location?
### walkthrough
mình search "motogp indonesia bar" và nó hiện ra 1 link facebook

<img width="1100" height="446" alt="Screenshot 2026-09-19 223400" src="https://github.com/user-attachments/assets/83cc5aa5-526d-404e-a484-1535a7417b83" />

rồi mình tra địa chỉ của bar trên google map, theo định dạng đúng của flag thì mình lược bớt 1 số thông tin

<img width="1222" height="680" alt="Screenshot 2026-09-19 23554" src="https://github.com/user-attachments/assets/058aa0e9-72f9-4ef8-9937-6fa64276f5be" />

## flag
`Jl. Raya Kuta, Kuta, Kec. Pujut, Kabupaten Lombok Tengah, Nusa Tenggara Bar`
---
## 6.
> What is the DJ's stage name?
### walkthrough
cũng là cùng cái link facebook đó có luôn thông tin về stage

<img width="1100" height="446" alt="Screenshot 2026-09-19 223400" src="https://github.com/user-attachments/assets/90836be2-f0fa-4c90-a7a3-1ced56220b5b" />

## flag
`Bong Leleh`
---
## 7.
> After digging into the DJ's other online accounts, what cave does he take tourists to?
### walkthrough
mình tìm những cái cave gần bar đó trên google map, thử từng cái, rất may là thử cái đầu tiên thì trúng luôn lmao :))

<img width="1227" height="689" alt="Screenshot 2026-09-19 22304" src="https://github.com/user-attachments/assets/40e0c728-76e2-4691-b312-7bc17d0bbc80" />

## flag
`Gua Sumur`
---
## 8.
> What number did the DJ list for his tour business?
### walkthrough
mình lại tìm tiếp tên của cave trên ở facebook và nó ra 1 cái page, trong đó để luôn number ở phần giới thiệu trang, theo như định dạng của flag thì mình sẽ bỏ đi số vùng ở đầu

<img width="1095" height="656" alt="Screenshot 2026-09-19 22487" src="https://github.com/user-attachments/assets/2208fe04-59ba-4aed-9d7e-199d3c50b108" />

## flag
`085333137345`
