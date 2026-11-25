```java
public class Profile {

    String name = "Vidhanshu Kelawala";
    String role = "Backend & AI Agents Engineer";
    String base = "M.Sc. Information Technology @ Somaiya Vidyavihar University";

    String[] interests = {
        "Distributed Systems",
        "Backend Engineering",
        "Agentic AI & RAG",
        "System Design",
        "Performance Engineering"
    };

    String[] languages = {
        "Java", "Python", "JavaScript", "C++", "SQL"
    };

    String[] currentFocus = {
        "Multi-agent PR review — LangGraph, MCP, RAG",
        "Implementing distributed systems from scratch: Raft, replication, storage",
        "Microservices with Spring Cloud, Kafka and OAuth2"
    };

    Project[] projects = {
        new Project("AI-Powered PR Reviewer",
                    "Multi-agent GitHub App — Spring Boot MCP server + LangGraph agents with a Critic",
                    "Java, Spring Boot, Spring AI, Python, FastAPI, pgvector"),
        new Project("QueueForge",
                    "Kafka-style message queue over raw TCP — Raft election, ISR acks, ~50x faster appends",
                    "Java, Custom TCP Protocol, Raft"),
        new Project("FitPro",
                    "6-service microservices app — Kafka events, Keycloak/JWT at the gateway",
                    "Java, Spring Cloud, Kafka, MongoDB, PostgreSQL")
    };

    TechStack tech = new TechStack();
    static class TechStack {
        String[] backend = {
            "Spring Boot", "Spring Cloud", "Spring AI", "Hibernate/JPA",
            "FastAPI", "REST APIs", "Microservices", "Kafka", "Resilience4j"
        };

        String[] data = {
            "PostgreSQL (pgvector)", "MySQL", "MongoDB", "Redis"
        };

        String[] ai = {
            "RAG", "LangGraph", "LangChain", "LangSmith",
            "Model Context Protocol (MCP)", "Agentic Workflows"
        };

        String[] infra = { "Docker", "Docker Compose", "Git", "Maven" };
    }

    record Project(String name, String what, String stack) {}
}
```