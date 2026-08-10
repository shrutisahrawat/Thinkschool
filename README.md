# Day 1 — Hello in Two Languages

Same tiny program, written two ways — comparing a runtime with heavy upfront structure (.NET) against one with none (Node/TypeScript).

## Structure
day-1/
├── hello-cs/ # C# console app
│ ├── Program.cs
│ └── hello-cs.csproj
└── hello-ts/ # TypeScript file
└── hello.ts
## Running hello-cs (C#)

```bash
cd hello-cs
dotnet run
```

Output: `Hello, Shruti`

## Running hello-ts (TypeScript)

```bash
cd hello-ts
node hello.ts
```

Output: `Hello, Shruti`

Node 24 runs `.ts` files directly — no `tsc` compile step needed.

## What surprised me

C# scaffolds a full project automatically — a `.csproj` XML file specifying the SDK, target framework, output type, and nullable settings — just to run one line of code. TypeScript on Node 24 needed nothing: no config file, no compile step, no project structure at all. One runtime hands you structure and conventions upfront; the other trusts you to bring your own.

## Tools

- .NET SDK 10
- Node 24 LTS
