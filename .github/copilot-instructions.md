# Copilot Instructions for EmpowerH

## Project Overview

EmpowerH is a comprehensive web platform dedicated to addressing sexual and gender-based violence (SGBV), domestic abuse, and mental health challenges. The platform provides:

- Anonymous reporting system for victims of violence
- Mental health support services and resources
- Wellness hub with health tips and reminders
- Community discussion and support forums
- Educational resources on rights, legal awareness, and self-protection

## Project Structure

```
EmpowerH/
├── frontend/          # Vue.js 3 application
│   ├── src/
│   │   ├── views/    # Vue components for pages
│   │   ├── assets/   # Static assets (CSS, images)
│   │   └── router/   # Vue Router configuration
│   ├── public/       # Public static files
│   └── package.json  # Frontend dependencies
├── CONTRIBUTING.md   # Contribution guidelines
├── CODE_OF_CONDUCT.md
└── README.md
```

## Technology Stack

### Frontend
- **Vue.js 3**: Progressive JavaScript framework
- **Vite**: Build tool and development server
- **Vue Router**: Client-side routing
- **Axios**: HTTP client for API requests
- **HTML5/CSS3**: Markup and styling
- **JavaScript (ES6+)**: Programming language

### Planned Backend (not yet implemented)
- Python with FastAPI
- SQLAlchemy ORM
- SQLite database

## Development Guidelines

### Code Style

1. **Vue Components**
   - Use Vue 3 Composition API where appropriate
   - Keep components focused and single-purpose
   - Use meaningful component and variable names
   - Follow Vue.js style guide conventions

2. **JavaScript**
   - Use ES6+ features (arrow functions, async/await, destructuring)
   - Use camelCase for variables and functions
   - Use PascalCase for component names
   - Add comments for complex logic

3. **CSS**
   - Use existing CSS variables defined in `main.css`
   - Follow mobile-first responsive design
   - Maintain consistency with existing styling patterns
   - Support dark theme using `.dark-theme` class

4. **File Organization**
   - Place new Vue views in `frontend/src/views/`
   - Place reusable components in `frontend/src/components/`
   - Place static assets in `frontend/src/assets/`

### Contribution Workflow

1. **Branching Strategy**
   - `main` branch: Stable production code
   - `frontend` branch: Frontend development
   - `backend-py` branch: Backend development (when implemented)
   - Feature branches: `feature/description` or `fix/description`

2. **Pull Request Targets**
   - Frontend contributions → `frontend` branch
   - Backend contributions → `backend-py` branch
   - Documentation/other → `main` branch

3. **Before Making Changes**
   - Review CONTRIBUTING.md for detailed contribution steps
   - Open an issue to discuss significant changes
   - Fork the repository and create a feature branch
   - Keep commits focused and atomic

### Testing and Building

```bash
# Install dependencies
cd frontend
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

### Important Considerations

1. **Privacy and Security**
   - This platform handles sensitive user data about violence and mental health
   - Always prioritize user privacy and data security
   - Use secure authentication and authorization patterns
   - Never expose sensitive information in logs or error messages

2. **Accessibility**
   - Ensure the platform is accessible to users with disabilities
   - Use semantic HTML elements
   - Provide alt text for images
   - Ensure keyboard navigation works properly

3. **Inclusive Language**
   - Use gender-neutral and inclusive language (e.g., "individuals", "people", "survivors" rather than gender-specific terms)
   - Be sensitive to the trauma victims may have experienced
   - Follow the CODE_OF_CONDUCT.md guidelines
   - Reflect the platform's commitment to serving all individuals regardless of gender identity

4. **Mobile-First Design**
   - The platform should work well on mobile devices
   - Test responsive layouts at various screen sizes
   - Consider touch-friendly interface elements

## Common Tasks

### Adding a New Page

1. Create a new Vue component in `frontend/src/views/`
2. Add the route in the router configuration
3. Update navigation links if needed
4. Ensure the page follows the existing design patterns

### Updating Styles

1. Use existing CSS variables from `frontend/src/assets/main.css`
2. Follow the mobile-first approach
3. Test both light and dark themes
4. Maintain consistency with existing pages

### Working with API Calls

1. Use Axios for HTTP requests
2. Handle loading states appropriately
3. Implement proper error handling
4. Show user-friendly error messages

## Resources

- [Vue.js Documentation](https://vuejs.org/)
- [Vite Documentation](https://vitejs.dev/)
- [Vue Router Documentation](https://router.vuejs.org/)
- [GitHub Best Practices for Copilot](https://gh.io/copilot-coding-agent-tips)

## Questions?

- Check existing issues in the repository
- Review CONTRIBUTING.md for contribution guidelines
- Open a new issue for questions or discussions
- Follow the CODE_OF_CONDUCT.md in all interactions
