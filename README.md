## Simple EQ

<p>A free, open-source 3-band equalizer audio plugin with a real-time spectrum analyzer and response curve display, built using the JUCE framework.<p>

<p>The plugin is available as Windows VST3, macOS VST3, and macOS AU formats.<p>

<img src="https://github.com/user-attachments/assets/7cf3e679-8b7d-4a35-99b1-08b59001f2b8" width="600" height="500">

## Features

<ul>
  <li><strong>3-Band Equalizer</strong>: Low, Mid, and High frequency bands with adjustable gain and Q controls.</li>
  <li><strong>Spectrum Analyzer</strong>: Visualize the frequency spectrum of the incoming audio signal.</li>
  <li><strong>Response Curve Display</strong>: Real-time graph of the filter response, aiding precise tonal adjustments.</li>
  <li><strong>Low CPU Footprint</strong>: Efficient DSP implementation for smooth performance in any DAW.</li>
  <li><strong>Precompiled Binaries</strong>: Ready-to-use plugin files included for Windows VST3, macOS VST3, and macOS AU.</li>
  <li><strong>Open Source</strong>: Full source code available.</li>
</ul>

## Repository

---

Clone this fork:

```bash
git clone https://github.com/LarreaSound/SimpleEQ.git
cd SimpleEQ 
```

## This repo contains:

SimpleEQ.jucer — the Projucer project file

SimpleEQ.filtergraph — DSP filter-graph definition

(On export) Build/ — your IDE project files and source code folders

## Prerequisites

JUCE 6+ [JUCE](https://juce.com/)

A C++17-capable compiler (Visual Studio, Xcode, CLang, GCC)

Projucer (to open ```.jucer```)

## Building
Open ```SimpleEQ.jucer``` in Projucer

Set your desired plugin formats (e.g. VST3, AU) in the <strong>Project Settings → Exporters</strong>

Save and Export to generate IDE project files

Open the generated project in your IDE

Build the ```Plugin``` target

## Usage
Load the built plugin in your DAW or audio host

Adjust Low, Mid, High bands (gain, frequency & Q)

Observe the Spectrum Analyzer and Response Curve updating in real time

## Project Structure

SimpleEQ/

├── .gitignore

├── SimpleEQ.jucer              # JUCE Projucer project

├── SimpleEQ.filtergraph        # DSP filter-graph file

├── Builds/                     # (auto-generated) IDE export folders

│     ├── VisualStudio2022/

│     ├── Xcode/

│     └── …

└── Source/                     # (auto-generated) .cpp / .h plugin sources

## Credits
Original Plugin & Tutorial by [Matkat Music](https://www.programmingformusicians.com/) (PFM::SimpleEQ) 

Recreated by Julio Larrea / LarreaSound (2025)
