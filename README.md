# 📘 BlazorComponentComms

A demo Blazor application showcasing **component communication patterns** in both **Blazor WebAssembly** and **Blazor Server**.

---

## 🔧 Features

This project demonstrates three key ways Blazor components communicate:

| Page             | Communication Pattern | Description                           |
|------------------|-----------------------|---------------------------------------|
| `/event-callback` | `EventCallback`       | Child notifies parent of an event     |
| `/cascading`      | `CascadingParameter`  | Shared model with reactive changes    |
| `/ref-example`    | `@ref`                | Parent calls child methods directly   |

---

## 🧪 Tech Stack

- Blazor WebAssembly or Blazor Server
- .NET 6 / 7 / 8
- Bootstrap 5 for basic styling

---

## ▶️ Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/stevsharp/BlazorComponentComms.git
   cd BlazorComponentComms

🧠 Learnings

📤 EventCallback: Raise events from child to parent

🌐 CascadingParameter: Share models down the tree (with reactivity)

📞 @ref: Access child methods directly from the parent

✍️ ValueChanged: Fine-grained control over data binding

🔄 Update with StateHasChanged()
