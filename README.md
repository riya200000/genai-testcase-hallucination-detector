# genai-testcase-hallucination-detector
Detects hallucinations in GenAI-generated test cases using Java, Spring Boot, and rule-based validation.
This project demonstrates how Generative AI can introduce hallucinations in software testing and how a tester-driven, rule-based validation system can detect and control them.

The application generates test cases using GenAI and validates them against strictly scoped functional requirements, flagging any out-of-scope assumptions with severity levels.

The project is inspired by real-world e-commerce flows (search, product details, add to cart).
🧪 Validation Rules (Examples)


🛠️ Tech Stack
Backend
Java 17
Spring Boot
Maven
GenAI
OpenAI / Gemini API (via REST)
UI
Thymeleaf
HTML / CSS
Testing
JUnit 5

Rule-based validation tests

📁 Project Structure
genai-testcase-hallucination-detector/
├── controller/
├── service/
│   ├── AiTestGeneratorService.java
│   ├── HallucinationDetector.java
│   └── ValidationService.java
├── parser/
├── model/
├── templates/
│   ├── index.html
│   └── result.html
├── test/
└── README.md
🧪 Testing Strategy

Unit tests for hallucination rules
Validation tests for false positives
Boundary cases (partial requirements)
Mixed severity test cases

⚠️ Limitations

Rule-based detection (no ML model)
Depends on requirement clarity
Keyword-based matching in initial version
