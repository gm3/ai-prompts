# Ultimate AI Coding Assistant Ruleset for Unity Development

## Core Principles
- Write clean, simple, readable code with minimal lines
- Think before coding - start with 2-3 reasoning paragraphs
- Implement features using the simplest possible approach
- Keep files small and focused (<200 lines)
- Use clear, consistent naming conventions
- Focus on core functionality before optimization
- Test after every meaningful change

## Prompting Strategies
- "Proceed like a senior developer" when seeking high-quality implementations
- "Do not stop until complete" for comprehensive solutions
- "Start with uncertainty" to encourage thorough analysis
- "Three reasoning paragraphs" before solving problems
- "Answer in short" when brevity is needed
- "Summary of current state" to track progress factually
- "Unbiased 50/50" for comparing alternative approaches
- "Be careful with red herrings" to stay focused on relevant information
- "Only include truly necessary steps" for efficient implementations
- "Properly formed search query" for effective research

## Error Handling
- DO NOT JUMP TO CONCLUSIONS! Consider multiple possible causes
- Explain problems in plain English first
- Make minimal necessary changes, modifying as few lines as possible
- For strange errors, perform web searches for up-to-date information

## Documentation
- ALWAYS add helpful and explanatory comments
- NEVER delete old comments unless obviously wrong/obsolete
- Document all changes and their reasoning in comments
- Use clear, easy-to-understand language in short sentences
- Verify each feature works by providing testing instructions

## Style Guidelines
- Simple over complex
- Clean over clever
- Modular over monolithic
- Readable over condensed
- Well-documented over assumed knowledge

## Unity-Specific Stack Guidelines
- Organize scripts in meaningful directory structures (Controllers, Models, Views, Utilities, etc.)
- Follow Unity's component-based architecture - one behavior per component
- Prefer [SerializeField] private variables over public fields
- Use ScriptableObjects for configuration data and shared resources
- Implement robust event systems instead of direct references (UnityEvents, C# events, or ScriptableObject events)
- Use interfaces for dependency injection and easier testing
- Implement proper singleton patterns when absolutely necessary
- Separate UI logic from game logic
- Cache component references in Awake() for better performance
- Use coroutines for time-based operations, not Update()
- Implement proper object pooling for frequently instantiated objects
- Use addressables for asset management in larger projects
- Follow Unity's execution order (Awake > OnEnable > Start > Update)
- Utilize custom editors and property drawers for better workflow
- Implement proper state machines for complex behavior
- Use extension methods for common Unity operations
- Implement proper input handling with the new Input System
- Prefer composition over inheritance
- Write editor tests for critical systems
- Use RequireComponent attribute for dependencies
- Implement proper scene management for modular loading
- Optimize shader code for target platforms
- Use UniTask for async/await pattern in Unity
- Handle null references with GetComponent checks or [RequireComponent]
- Implement proper error handling with try/catch in editor scripts
- Use appropriate collider types for physics interactions
- Structure prefabs hierarchically with nested prefab variants
- Follow Unity's recommended performance optimization guidelines
- Implement proper memory management with Resources.UnloadUnusedAssets()
- Use Jobs system and Burst compiler for performance-critical code
- Implement proper localization systems using built-in or asset store solutions
- Use animation state machines effectively for complex animations
- Document public API with XML comments
