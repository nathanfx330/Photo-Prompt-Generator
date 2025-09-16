# Photo Prompt Generator

## Description

**Photo Prompt Generator** is a simple, single-file HTML and JavaScript application that provides a user-friendly interface to generate structured JSON objects and descriptive natural language prompts. These prompts are designed to be fed into an AI or LLM (Large Language Model) image generator to create realistic and period-accurate photos.

This tool bridges the gap between a creative idea (e.g., *"a girl on a boat"*) and the detailed, specific instructions an AI needs to produce a high-quality, targeted image.

---

## Features

- **User-Friendly Interface:** Clean and simple web interface with dropdowns and text fields for easy input.  
- **Detailed Shot Parameters:** Define everything from the subject and location to camera angles, shot types, time of day, and lighting.  
- **Era-Specific Details:** Generate photos with the aesthetic of different decades, from the 1950s to modern times.  
- **Selfie Perspective & Full Body:** Includes options for "selfie perspective" and "full body" shots for more control.  
- **Dual Output:** Generates both a structured JSON object (for programmatic use) and a human-readable LLM prompt.  
- **Dark Theme:** Easy on the eyes for comfortable use.  
- **Zero Dependencies:** Runs entirely in the browser. No installation or setup required.  

---

## How to Use

1. **Download the File:** Save the `[your_file_name].html` file to your local computer.  
2. **Open in Browser:** Open the HTML file with any modern web browser (Chrome, Firefox, Edge, etc.).  
3. **Fill in the Details:**  
   - Start with a **Subject/Scene** description.  
   - Select the desired **Camera Angle**, **Shot Type**, **Time of Day**, and **Lighting Style**.  
   - Choose the **Era/Period** for a vintage or modern feel.  
   - (Optional) Add more details about the location, mood, or overall aesthetic.  
4. **Generate:** Click the **"Generate Description"** button.  
5. **Copy and Use:**  
   - The **Generated JSON** appears in the first output box — ideal for API calls or logging settings.  
   - The **Generated LLM Prompt** appears in the second text area — copy it into your AI image generator (e.g., MidJourney, DALL-E 3, Stable Diffusion).  

---

## What It Solves

AI image generators require very specific prompts for the best results. Writing all the parameters manually is time-consuming and error-prone. This tool helps you:

- **Improve Consistency:** Easily regenerate prompts with minor variations.  
- **Save Time:** Quickly build complex prompts without remembering all technical terms.  
- **Enhance Creativity:** Experiment with different camera and lighting setups to discover new visual styles.  

---

## Future Enhancements

- **Direct API Integration:** Connect directly to image generation APIs to generate and display photos within the application.  
- **Preset Templates:** Save and load templates for common shot types (e.g., "Cinematic Portrait," "Vintage Family Photo").  
- **Visual Previews:** Show example images that correspond to different settings to guide the user’s choices.  

---

## Technology Stack

- **HTML:** Structure and layout of the application.  
- **CSS:** Dark theme styling and responsiveness.  
- **JavaScript:** Core logic for collecting user input and generating JSON and prompts.  

---

## Example Output

**User Input:**

```text
Subject/Scene: A man standing on a neon-lit street corner in Tokyo
Camera Angle: Low-angle shot
Shot Type: Full shot (Full Body)
Time of Day: Night
Lighting Style: Cinematic lighting
Era/Period: 1980s
````

**Generated JSON:**

```json
{
  "subject_scene": "A man standing on a neon-lit street corner in Tokyo",
  "camera": {
    "angle": "low-angle",
    "shot_type": "full-shot"
  },
  "environment": {
    "time_of_day": "night",
    "lighting_style": "cinematic",
    "era_period": "1980s"
  }
}
```

**Generated LLM Prompt:**

```
A man standing on a neon-lit street corner in Tokyo, reflecting 1980s photographic trends. Full shot (Full Body) from a low-angle perspective. The subject's full body is visible. Time of day: Night. Lighting: Cinematic lighting. High-resolution, photorealistic.
```

