# maven-index

This repository stores the index of Java packages published on [Maven Central Repository](https://repo.maven.apache.org/maven2).
It provides a searchable and usable collection of metadata for Java packages available in the central repository.

## SHA1 Shard Lookup

Artifacts are sharded across multiple TSV files for efficiency.
To find the shard for a given group ID and artifact ID, use the web interface at https://aquasecurity.github.io/maven-index/.
It computes the FNV-1a hash of the identifiers and automatically redirects you to the corresponding shard file in the `central` directory.

## Automatic Updates

This repository has a GitHub Action configured to automatically update the Maven index using [trivy-java-db](https://github.com/aquasecurity/trivy-java-db).

Updates are performed at the following times:
- Automatically every day at midnight (UTC)
- Manually when the workflow is triggered
