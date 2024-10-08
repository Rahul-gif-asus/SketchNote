# SketchNote

### A Rich Text & Diagramming Tool

SketchNote is an innovative web application that seamlessly integrates **rich text editing** with **diagramming** capabilities, providing users with a versatile tool for note-taking, brainstorming, and project planning. Built using modern JavaScript and open-source libraries like **Quill.js** and **tldraw**, it allows users to easily switch between creating rich text content and visual diagrams. The project is hosted on Firebase, utilizing its free tier for backend functionality such as user authentication and cloud storage.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Setup Instructions](#setup-instructions)
- [Folder Structure](#folder-structure)
- [Light/Dark Mode](#light-dark-mode)
- [Future Enhancements](#future-enhancements)
- [Collaborative Editing](#collaborative-editing)
- [Roadmap](#roadmap)
- [License](#license)

---

## Project Overview

SketchNote combines two powerful tools:
1. **Quill.js** for rich text editing (text formatting, lists, links, images).
2. **tldraw** for creating diagrams (flowcharts, mind maps, sketches).

This synergy provides an all-in-one solution for individuals looking to enhance their productivity by keeping their notes and visual ideas in one place. **SketchNote** is ideal for students, professionals, or anyone who needs a blend of text and visual elements in their documentation.

---

## Features

- **Rich Text Editing**:
  - Bold, italic, underline, headings, links, bullet points.
  - Embedding images, videos, and media into notes.
  - Full keyboard shortcuts for faster note-taking.

- **Diagramming**:
  - Drawing tools like lines, arrows, rectangles, and more using **tldraw**.
  - Moving, resizing, and grouping diagram elements.
  - Exporting diagrams to PNG, JPEG, or SVG.

- **Light/Dark Mode**:
  - User-friendly light and dark mode toggle at the top of the interface.

- **Cloud Storage**:
  - Notes and diagrams can be saved to Firebase's Firestore, allowing users to access their work from anywhere.

- **Undo/Redo**:
  - History management to allow users to undo/redo actions for both text and diagrams.

- **Collaborative Editing (Planned)**:
  - Real-time collaboration where multiple users can edit text and diagrams together (future enhancement).

---

## Technology Stack

### Frontend:
- **React.js**: For building a dynamic user interface.
- **Quill.js**: Rich text editor.
- **tldraw**: For creating diagrams.
- **Material UI (MUI)**: For UI components and responsive design.
- **CSS3**: For custom styling and animations.
- **Firebase Hosting**: For hosting the app and managing cloud functionalities.

### Backend:
- **Firebase Firestore**: To store user notes and diagrams in real-time.
- **Firebase Authentication**: To manage user logins (optional feature for the end).
  
### Additional:
- **Chart.js** (Optional): For future integration of data visualization.
- **Framer Motion**: For animations and smooth transitions.
- **Redux or Zustand**: To manage the app’s global state efficiently.

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/SketchNote.git
   ```
   
2. Navigate into the directory:
   ```bash
   cd SketchNote
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Set up Firebase:
   - Go to the Firebase console, create a new project, and enable Firestore.
   - Enable Firebase Authentication if you plan to implement login functionality.
   - Add the Firebase configuration in a `.env.local` file.
   
5. Run the app:
   ```bash
   npm run dev
   ```

---

## Folder Structure

```
/src
  /components
    RichTextEditor.js      // Rich text editor using Quill.js
    DiagramEditor.js       // Diagram editor using tldraw
    Toolbar.js             // Common toolbar for text and diagram controls
  /pages
    index.js               // Main app entry point
  /utils
    firebaseConfig.js      // Firebase configuration
  /styles
    global.css             // Global CSS and theming
  App.js                   // Main component integrating both editors
README.md
package.json
```

---

## Light/Dark Mode

SketchNote includes a light and dark mode toggle to enhance user experience in different environments. The toggle is positioned in the header, and the app adjusts the UI colors accordingly to suit the selected mode.

---

## Future Enhancements

- **Real-time collaboration**: Enable multiple users to work together simultaneously.
- **User authentication**: Login and registration using Firebase Authentication for saving individual user’s work.
- **Export options**: Allow users to export notes and diagrams as PDFs or images.
- **Version control**: Track changes made to notes and diagrams over time, allowing users to revert back to previous versions.

---

## Collaborative Editing

In the future, SketchNote will include collaborative editing functionality where multiple users can work on the same document simultaneously. Firebase Realtime Database will manage document changes in real-time, keeping all participants in sync.

---

## Roadmap

1. **Initial Build**: Set up Quill.js and tldraw integration.
2. **UI Design**: Implement MUI components for a professional look.
3. **Light/Dark Mode**: Implement theme switcher.
4. **Cloud Integration**: Store notes and diagrams in Firebase Firestore.
5. **Optional Features**: Add collaborative editing and user authentication.

---

## License

This project is licensed under the MIT License.

---

## Fonts, Colors & Themes

- **Primary Font**: Roboto (MUI default) for readability.
- **Heading Font**: Montserrat for modern, clean headers.
- **Colors**:
  - **Light Mode**: Clean whites with subtle gray tones for a fresh look.
  - **Dark Mode**: Dark blues and grays for minimal eye strain.

---

## Conclusion

SketchNote is designed to be a robust, easy-to-use tool for combining rich text and diagramming capabilities. The aim is to provide an intuitive yet powerful interface for users to create content that merges text and visuals seamlessly.
Let me know how you'd like to proceed and what you'd like to tackle first!
