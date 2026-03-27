# lab1-terraform

[![Terraform CI](https://github.com/Oshansheru/lab1-terraform/actions/workflows/terraform.yml/badge.svg)](https://github.com/Oshansheru/lab1-terraform/actions/workflows/terraform.yml)

# Lab 1 – Terraform VM on GCP

This project uses Terraform to create a Linux VM in Google Cloud Platform (GCP). The VM uses Ubuntu 22.04 and includes basic hardening with `ufw`, `fail2ban`, and `unattended-upgrades`. The project also includes a daily snapshot backup policy and a GitHub Actions pipeline for formatting, security scanning, and Terraform validation.

# How to run the code

first run : terraform init 

then run : terraform plan

it will plan out what terraform code will do

and lastly run : terraform apply

# screenshot of pipeline

<img width="937" height="405" alt="Skärmbild 2026-03-11 123719" src="https://github.com/user-attachments/assets/e71fd03a-998e-48f2-b310-dc341848ee9e" />

# screenshot of working vm

<img alt="Skärmbild" src="assets/Skärmbild 2026-03-13 215559.png"/>

# screenshot of error 403 when trying to apply backup policies

<img alt="Skärmbild" src="assets/Skärmbild 2026-03-24 195549.png"/>

## Security decisions

This VM includes a few basic security measures to reduce risk and improve system safety. `ufw` is used as a simple firewall to block unwanted incoming traffic while still allowing SSH access. `fail2ban` helps protect the server from repeated login attempts, especially against brute-force attacks on SSH. `unattended-upgrades` is installed to automatically apply important security updates so the system stays patched. A daily snapshot backup policy is also included to improve recovery in case something goes wrong with the VM or disk.

# #meafterimdone
![Pipeline demo](assets/seal-spinning-around.gif)
