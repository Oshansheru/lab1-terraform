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
