# 📘 BlazorComponentComms

A demo Blazor application showcasing **component communication patterns** in both **Blazor WebAssembly** and **Blazor Server**.

## 🔧 Features

This project demonstrates three key ways Blazor components communicate:

| Page             | Communication Pattern | Description                           |
|------------------|-----------------------|---------------------------------------|
| `/event-callback` | `EventCallback`       | Child notifies parent of an event     |
| `/cascading`      | `CascadingParameter`  | Shared model with reactive changes    |
| `/ref-example`    | `@ref`                | Parent calls child methods directly   |

## 🧪 Tech Stack

- Blazor WebAssembly or Blazor Server
- .NET 6 / 7 / 8
- Bootstrap 5 for basic styling

## ▶️ Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/stevsharp/BlazorComponentComms.git
   cd BlazorComponentComms


---

## ▶️ Getting Started

1. Clone this repo:

   ```bash
   git clone https://github.com/stevsharp/BlazorComponentComms.git
   cd BlazorComponentComms

✍️ Code Overview (Inside Index.razor)
razor
Copy
Edit
<InputText
    Value="p.Name"
    ValueChanged="(string val) => OnNameChanged(p, val)"
    ValueExpression="() => p.Name" />
csharp
Copy
Edit
private void OnNameChanged(Product p, string val)
{
    p.Name = val;
    changedIds.Add(p.Id);
}
🧠 Learnings
How to use ValueChanged instead of @bind for full control

How to track changes to specific objects in a list

Use of @ref to access child logic from parent

🤝 Contributions
Feel free to open a PR to expand this demo with:

EventCallback version

CascadingParameter version

Visual diffing and row highlighting
