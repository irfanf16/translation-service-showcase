# Translation Service — Localisation Microservice

**Microservice · Laravel + Docker**

A small, single-purpose HTTP service providing translation and locale management to other applications.

> **Source code is private.** This repository documents the architecture and engineering work.

## My role
Backend engineer

## Engineering highlights

**Extracted as a service.** Translation was duplicated across several products; pulling it into one Sanctum-authenticated HTTP service meant a single translation cache and one place to change providers, instead of the same integration re-implemented per app.

**Deliberately small.** Laravel framework, Sanctum and Tinker only — no ORM plugins, no UI libraries. A service with one job keeps its dependency surface proportional.

**Containerised.** docker-compose definition for drop-in deployment alongside consuming services.



## Stack

`Laravel` · `PHP` · `Sanctum` · `Docker` · `Blade`
