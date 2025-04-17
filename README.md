# maven-index

This repository stores the index of Java packages published on [Maven Central Repository](https://repo.maven.apache.org/maven2).
It provides a searchable and usable collection of metadata for Java packages available in the central repository.

## Automatic Updates

This repository has a GitHub Action configured to automatically update the Maven index using [trivy-java-db](https://github.com/aquasecurity/trivy-java-db).

Updates are performed at the following times:
- Automatically every day at midnight (UTC)
- Manually when the workflow is triggered
