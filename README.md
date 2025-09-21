# Travel Journal (React)

Learning project: a React-based travel journal app built with **React and Vite**.  
Created to practice **component architecture, props, data mapping, reusable components, modular project structure, and responsive CSS design**.

## 🚀 Features
- **Header** with globe icon and project title  
- **Dynamic travel entries** generated from `data.js` including:  
  - Location image  
  - Country name and map marker icon  
  - Direct link to Google Maps for the location  
  - Title, trip dates, and descriptive text  
- **Reusable Entry component** for each travel log  
- **Props spreading** to pass data cleanly into components  
- **Flexbox-based responsive layout** for consistent styling  
- Organized structure with separate components, data, and assets  

## 🛠️ Tech Stack
- React 19 (RC)  
- Vite  
- JavaScript (ES6+)  
- CSS3  

## 📂 Project Structure
```
travel-journal/
├── App.jsx               # Root component, renders Header + Entries
├── README.md             # Project documentation
├── components/           # React components
│   ├── Entry.jsx         # Individual travel entry card
│   └── Header.jsx        # Navbar/header with globe icon + title
├── data.js               # Travel entry data (location, dates, text, images)
├── images/               # Assets (globe + marker icons)
│   ├── globe.png
│   └── marker.png
├── index.css             # Global styles
├── index.html            # Root HTML template
├── index.jsx             # Entry point, renders <App />
├── package.json          # Project metadata and dependencies
└── vite.config.js        # Vite configuration
```

## ⚙️ How It Works
- `data.js` contains structured objects with properties: `id`, `img`, `title`, `country`, `googleMapsLink`, `dates`, and `text`.  
- `App.jsx` imports the data and uses `.map()` to render an `<Entry />` component for each item.  
- Each `Entry.jsx` receives props (spread via `{...entry}`) to dynamically display its details.  
- `Header.jsx` contains a static header with a globe icon and title.  
- Styling is handled in `index.css` with Flexbox for layout and spacing.  
- Images are stored in the `images/` folder and referenced in components.  

## 📈 Learning Purpose
This project helped me practice:  
- Building a **React app from scratch with Vite**  
- Using **functional components** and separating concerns into files  
- **Passing props** and using the spread operator to simplify component rendering  
- **Mapping over data arrays** to dynamically generate UI elements  
- Managing a clean **component hierarchy** (`App → Header + Entry list`)  
- **Organizing assets and data** into a modular file/folder structure  
- Writing **responsive CSS** with Flexbox to adapt layout  
- Understanding how React projects are scaffolded with **Vite configuration**  

---

⚠️ **Note**: This was built purely as a **learning project** and is not intended for production use.
