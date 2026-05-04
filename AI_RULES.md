# AI Rules & Guidelines

## Tech Stack
* **Framework**: React (using TypeScript)
* **Routing**: React Router (routes are strictly maintained in `src/App.tsx`)
* **Styling**: Tailwind CSS
* **UI Library**: shadcn/ui (built on top of Radix UI primitives)
* **Icons**: lucide-react
* **State Management**: Native React Hooks (e.g., `useState`, `useContext`)
* **Project Structure**: Pages belong in `src/pages/` and components belong in `src/components/`. The main entry page is always `src/pages/Index.tsx`.

## Library Usage Rules
* **Styling**: Exclusively use Tailwind CSS utility classes for all styling, layout, spacing, and colors. Avoid writing custom CSS files or using inline style attributes.
* **UI Components**: Rely on the pre-installed shadcn/ui components for building blocks. Do not edit the core shadcn/ui files directly; if you need to alter functionality, wrap them in a new custom component.
* **Icons**: Use `lucide-react` for all standard iconography across the application.
* **Routing**: Use `react-router-dom` components (`Link`, `useNavigate`, etc.) for internal navigation. All route definitions must stay in `src/App.tsx`.
* **Notifications**: Use standard toast notifications (like `react-hot-toast` or shadcn's toaster) to surface success states, errors, and system warnings to the user.
* **Component Architecture**: Create small, focused components (ideally under 100 lines of code). Always create a new `.tsx` file for every new component rather than adding multiple components to a single file. Keep directory names strictly lower-case.