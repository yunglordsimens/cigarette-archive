# ROMAN ROOM MONUMENT // DIGITAL ARCHIVE

FUCK THIS BULLSHIT IT DEOS NOT MAKE ANY SENSE THE POINT IS THAT I WAS COLLECTING SIGARRETE BOXES AND A LOT OF OTHER ACUAL PURE TRASH BECAUSE I WAS KEEPING EVERY MEMORY AS A TRESURE JUST BECAUSE I CAN REMEMBER EVERYTHING JUST BY LOOKING AT SOMTHING I COULDVE IMAGINE THE PICTURE HOW 10 YEARS AGO I WAS DOING WHAT I WAS DOING AND SMELLED EXACTLY WHAT I SMELLED FOR EX. . I JUST DECITED I AM NOT STORING TRASH ANYMORE NOT IN MY HEAD NOT IN (AS) MY PROPERTY. I WAS NOT MAKING BY HANDS A SHIT FOR A WHILE AND I ADORE IT. THE OTHER POINT IS THAT ITS A CROSS JUST BECOUSE IT WAS FIRT REFERANCE PICTURE I GOT TO REMEMBER WITH THIS TYPE OF SCULPURE I JUST LIKED THE PICTURE NOTHING SEEPER BEHINF IT 

<img src="./REF.png" width="100%" style="border-radius: 8px;">

An interactive 3D digital sculpture and personal manifesto. This project represents the final stage of letting go—transforming a 4-year physical collection of cigarette packs into a data-driven digital monument.

> ✝️ **"By building it, I am burying my past habit of hoarding and moving forward"**

🔗 **[View Interactive Sculpture](https://yunglordsimens.github.io/cigarette-archive/)**

---

### / VISUALIZATION

<img src="./preview_cross.gif" width="100%" alt="3D CSS Cross Interaction" style="border-radius: 8px; margin-bottom: 20px;">

---

### / THE MANIFESTO (Concept)

For years, I used physical objects—receipts, trinkets, empty packs—as memory anchors. My collection functioned as a **"Roman Room" (Method of Loci)**, where even the most insignificant piece of trash held a specific, vivid memory. 

In the past year, external catalysts deeply fractured this paradigm:
1. **Nomadism & Travel:** True comfort requires owning less.
2. **The Reality of War:** Emergency evacuations revealed the true value of belongings. Leaving behind expensive collections proved they were not life-sustaining. Life is more important than boxes.
3. **Rejecting "Deferred Life":** Abandoning the Soviet mindset of "saving the best for later." Things must be used here and now, or they lose their meaning.

This sculpture is a therapeutic act of separation. The physical material (cigarette packs) fulfilled its role by becoming art. By digitizing this archive into an interactive WebGL/CSS experience, I release the physical weight. **It is an act of liberation and a manifesto of living strictly in the present moment.**

---

### / TECH & ARCHITECTURE: "DATA AS MEMORY"

This isn't just a 3D model; it's a literal digitization of physical memory. Every single pack from the physical sculpture was audited, counted, and mapped into a JSON architecture (`CROSS_INVENTORY`). 

The application uses procedural generation to rebuild the physical object using code.

| Technology | Implementation Role |
| :--- | :--- |
| **React 19** | Core engine and state management. |
| **Vanilla CSS 3D** | Building the 3D shapes (prisms) purely through DOM manipulation (`transform: rotate3d`), bypassing heavy WebGL libraries for a raw, brutalist web aesthetic. |
| **Procedural Mapping** | The algorithm fetches objects from the data array (`takePack()`) mimicking the exact physical count and dimensions of the real-world items. |
| **Custom Camera** | Touch and mouse event listeners built from scratch to handle panning, pitching, and zooming in the 3D space. |

---

### / INTERFACE DETAILS

<table style="border: none; width: 100%;">
  <tr>
    <td width="50%" valign="top">
      <h4 align="center">THE ARCHIVE LIST</h4>
      <img src="./preview_list.png" width="100%" style="border-radius: 8px;">
      <p align="center"><i>Digital audit of the physical trash.</i></p>
    </td>
    <td width="50%" valign="top">
      <h4 align="center">FREE-ANGLE EXPLORATION</h4>
      <img src="./preview_rotate.gif" width="100%" style="border-radius: 8px;">
      <p align="center"><i>Custom CSS 3D camera controls.</i></p>
    </td>
  </tr>
</table>

---

## / LOCAL DEPLOYMENT

```bash
# Clone the archive
git clone [https://github.com/yunglordsimens/monument-to-debris.git](https://github.com/yunglordsimens/monument-to-debris.git)
cd monument-to-debris

# Install dependencies
npm install

# Run the digital sculpture
npm run dev
