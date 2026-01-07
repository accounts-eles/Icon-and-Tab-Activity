🗂️ Branded Icon and Tab Template

A premium, interactive tabbed interface built with Tailwind CSS. This component features a sophisticated branded color palette, circular icon placeholders, and responsive tab navigation, making it ideal for categorized content, service overviews, or multi-step documentation.

🚀 Live Demo

Explore the Tabbed Component Here

✨ Project Overview

The Branded Icon and Tab Template is designed to organize content into distinct, easily accessible categories. It prioritizes high-contrast visual cues through the use of specific brand colors and rounded UI elements that adapt seamlessly to different screen sizes.

Key Features

Dynamic Tab States: Buttons utilize specific background colors when inactive (Teal and Grey) and shift to a deep Midnight Blue when active, topped with a high-contrast accent border.

Icon-Centric Navigation: Each tab features a prominent circular container designed to hold icons or images, reinforcing the visual identity of each category.

Fluid Responsiveness: The navigation automatically stacks vertically on mobile devices and expands to a horizontal layout on tablets and desktops.

Accessible Visual Feedback: Uses a combination of background color shifts, border-bottom indicators, and text color changes to signal the active state.

Persistent Branding: A consistent color scheme applied via CSS variables ensures the UI remains cohesive regardless of the content displayed.

🛠️ Technical Implementation

Styling Engine: Tailwind CSS for layout utility combined with custom CSS variables for precise brand color mapping.

Typography: Leverages the Inter Google Font for a clean, modern aesthetic with optimized weight for readability.

Responsive Layout: Uses flexbox-based navigation with flex-col for mobile and sm:flex-row for larger viewports.

Visual Design Tokens:

Primary Dark (#1f2a52): Active tab backgrounds and primary headings.

Accent Light (#00bec7): Active borders and inactive backgrounds for Tabs 1 & 3.

Page Background (#d2f0f0): Soft aqua background for the entire page.

Secondary Grey (#abb5bf): Inactive background for Tab 2.

📂 Structure and Usage

The component is entirely self-contained within a single HTML file, optimized for rapid deployment.

Tab Navigation: A container holding button elements with data-tab attributes for state management.

Tab Content: Individual div blocks that toggle visibility based on the selected tab.

JavaScript Logic: A DOMContentLoaded listener manages the switching logic, ensuring smooth transitions between content sections.

function showTab(tabId) {
    // 1. Remove 'active' class from all buttons and content
    tabButtons.forEach(button => button.classList.remove('active'));
    tabContents.forEach(content => content.classList.remove('active'));

    // 2. Find and activate the corresponding button and content
    const activeButton = document.querySelector(`.tab-button[data-tab="${tabId}"]`);
    const activeContent = document.getElementById(tabId);

    if (activeButton) activeButton.classList.add('active');
    if (activeContent) activeContent.classList.add('active');
}


📄 License

MIT License - Developed as part of the accounts-eles UI component library.
