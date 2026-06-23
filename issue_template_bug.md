---
name: "🎨 UI Render Overflow Report"
about: Report layout clips, pixel overflows, or rendering artifacts across specific devices.
title: "ui: [Component Name] Right overflowed by X pixels"
labels: ["bug", "ui/ux", "render-overflow"]
assignees: ''
---

### 🛑 Layout Failure Summary
Provide a brief overview of what layout element is breaking and on which view layer.

### 📸 Visual Evidence
Attach screenshots, video clips, or GIFs highlighting the rendering issue.
> **Note:** Drag and drop your image directly below this line to embed it.


### 📲 Test Environment Details
* **Device / Screen Target:** (e.g., iPhone 17 Simulator, Physical Android Device)
* **OS / SDK Version:** (e.g., iOS 26.5, Android API 34)
* **App Build Channel:** Debug Mode / Profile Mode

### 🔍 Steps to Reproduce
Clear, sequential steps to navigate to the broken layout structure:
1. Open the application.
2. Navigate to the `______` module.
3. Advance to the `______` step/screen.
4. Look directly at the `______` component.

### 🧩 Affected Code Segment (If Known)
Paste the widget construction tree or code snippet that is causing the layout constraint failure:
```dart
// Insert snippet here (e.g., Row/Column setup missing Expanded widgets)
```

### 🎯 Expected vs. Actual Behavior
* **Expected:** The layout components scale down, truncate, or wrap safely to fit within the viewport boundaries without structural distortion.
* **Actual:** A layout exception is triggered (`RIGHT OVERFLOWED BY X PIXELS`), displaying the yellow-and-black striped debugger tape.

### 🛠 Suggested Resolution Strategy
Check whichever constraint adjustment strategy might fix this component:
- [ ] Wrap target text blocks or inner columns in an `Expanded` or `Flexible` layout widget.
- [ ] Enforce tight boundary truncations by passing `overflow: TextOverflow.ellipsis` to text strings.
- [ ] Reduce horizontal container padding rules (`EdgeInsets.symmetric`) to fit small viewports.
