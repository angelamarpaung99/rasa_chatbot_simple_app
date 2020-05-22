#### This file contains tests to evaluate that your bot behaves as expected.
#### If you want to learn more, please see the docs: https://rasa.com/docs/rasa/user-guide/testing-your-assistant/

## 1st story
* menyapa: hi
  - utter_greet
* konfirmasi_member: sudah
  - utter_ask_full_name
* name_entry : james
  - utter_ask_email 
* email_entry : james@gmail.com
  - action_member_form
  - utter_ask_phone_number
* phone_number_entry : 082946789993
  - utter_check_database
  - utter_db_found
  - utter_offer_plan
* minat_daftar : saya minat
  - utter_offer_paket
* paket_entry : 1
  - utter_link_pembayaran
  - utter_end_conversation

## 2nd story
* menyapa : halo
  - utter_greet
* menolak : belum
  - utter_link_registrasi
* tanya_harga : bayar berapa?
  - utter_offer_plan_registrasi
* minat_daftar : minat
  - utter_ask_full_name
* name_entry : angie
  - utter_ask_email 
* email_entry : angie@yahoo.com
  - action_member_form
  - utter_ask_phone_number
* phone_number_entry : +62812666994
  - utter_check_database
  - utter_db_found
  - utter_offer_plan
* minat_daftar : ya minat
  - utter_offer_paket
* paket_entry : paket 2
  - utter_link_pembayaran
  - utter_end_conversation

## 3rd story
* mencari_jodoh : saya ingin cari jodoh
  - utter_ask_criteria
* user_criteria : tinggi baik
  - utter_answer_criteria
* konfirmasi_member : sudah
  - utter_ask_full_name
* name_entry : katy
  - utter_ask_email
* email_entry : katy@gmail.com
  - action_member_form
  - utter_ask_phone_number
* phone_number_entry : +6281299957323
  - utter_check_database
  - utter_db_found
  - utter_offer_plan
* minat_daftar : minat
  - utter_offer_paket
* paket_entry : 1
  - utter_link_pembayaran
  - utter_end_conversation

## 4th story 
* mencari_jodoh : saya ingin cari jodoh
  - utter_ask_criteria
* user_criteria : baik
  - utter_answer_criteria
* menolak : belum
  - utter_link_registrasi
* tanya_harga: bayar berapa?
  - utter_offer_plan_registrasi
* minat_daftar : minat
  - utter_ask_full_name 
* name_entry : angie
  - utter_ask_email
* email_entry : angie@yahoo.com
  - action_member_form
  - utter_ask_phone_number
* phone_number_entry : 0812999387254
  - utter_check_database
  - utter_db_found
  - utter_offer_plan
* minat_daftar : minat
  - utter_offer_paket
* paket_entry : paket 1
  - utter_link_pembayaran
  - utter_end_conversation

## 5th story
* menyapa : selamat pagi
  - utter_greet 
* konfirmasi_member : sudah
  - utter_ask_full_name
* name_entry : reza
  - utter_ask_email
* email_entry: rezamarpaung@gmail.com
  - action_member_form
  - utter_ask_phone_number
* phone_number_entry : +628877753563
  - utter_check_database
  - utter_db_found
  - utter_offer_plan
* menolak : sepertinya tidak
  - utter_end_conversation

## 6th story 
* mencari_jodoh : saya pengen cari pasangan
  - utter_ask_criteria
* user_criteria : kriteria saya orangnya baik
  - utter_answer_criteria
* menolak : belum
  - utter_link_registrasi
* tanya_harga : berapa emangnya?
  - utter_offer_plan_registrasi
* menolak : tidak
  - utter_end_conversation
