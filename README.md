# ⏱️ Simple Timestamp Logger

[Live Demo on GitHub Pages](https://chuanchihsu1219.github.io/timestamp-logger/)

## Overview

This is a lightweight, user-friendly timestamp logging tool designed for real-world data collection tasks. Originally developed for a fieldwork assignment in the Operations Research course at National Taiwan University, the app was used to record human flow observations at Taipei 101.

Unlike existing timestamp tools that are often either overcomplicated or lack flexibility, this project focuses on:

* 👆 **Instant, easy one-click logging**
* 🧼 **Clean, distraction-free interface**
* 🧾 **Export logs in CSV with a single click**
* 💾 **Persistent local storage using `localStorage`**
* 🔄 **Automatic session recovery for seamless re-entry**

## Motivation

During our field data collection assignment, we discovered that most existing timestamp or note-taking tools were not built for rapid, repeated logging. Some required multiple clicks, had small interfaces, or lacked session continuity. Most tools also couldn't handle logging multiple events in quick succession, which was essential for recording dense foot traffic patterns at Taipei 101.

We needed a frictionless tool that supported:

* Ultra-fast and UX-friendly timestamping (even multiple times per second)
* Automatic saving of data across sessions
* Easy export of collected timestamps for downstream analysis

This gap motivated me to build a minimal yet powerful web app tailored specifically for high-frequency logging in real-world environments.

## Features

* 🎯 **Event Name Setup**
  Start by entering the name of the observation event.

* 🕒 **Timestamp Logging**
  Press the large central logging button to record the current timestamp (with milliseconds). The button is intentionally oversized for fast, accurate logging even on mobile devices or in distracting environments.

* 📜 **Live Log Display**
  Logged timestamps are displayed in real time and scroll automatically.

* 💾 **Session Persistence**
  All logs and settings are saved locally and automatically restored on reload.

* 📄 **Export to CSV**
  Export your timestamps to a clean CSV file with one click.

* ♻️ **Clear Data**
  Reset the current session with confirmation to avoid accidental deletion.

## Technical Stack

* 🧱 **Frontend**: Vanilla HTML, CSS, JavaScript
* 📦 **Storage**: `localStorage` for persistent logging
* 🚀 **Deployment**: GitHub Pages

> **Deployed App**: [https://chuanchihsu1219.github.io/timestamp-logger/](https://chuanchihsu1219.github.io/timestamp-logger/)

## Key Design Decisions

* **UX-first**: Designed to work on mobile and desktop, with centered button ergonomics for field usage.
* **Minimalist UI**: Reduces cognitive load in fast-paced environments like public space observations.
* **Offline-first**: Works without internet access once loaded.
* **Export logic**: CSV download includes event name and timestamp to facilitate data integration in OR modeling.

## Use Case: Human Flow Observation

This tool was used in a real-world case study to collect time-based human flow data at Taipei 101. Each timestamp represented a significant event, such as a person entering or exiting a zone. This allowed us to model and optimize queue systems and resource allocation using quantitative methods from Operations Research.

## Potential Applications

* Behavioral observation in public spaces
* Event marking during usability testing
* Logging milestones during manual testing
* Timestamped data for time-motion studies
