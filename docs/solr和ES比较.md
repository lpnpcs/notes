- 由于易于使用，Elasticsearch 在新开发者中更受欢迎。但是，如果您已经习惯了与 Solr 合作，请继续使用它，因为迁移到 Elasticsearch 没有特定的优势。

- 如果除了搜索文本之外还需要它来处理分析查询，Elasticsearch 是更好的选择。

- 如果需要分布式索引，则需要选择 Elasticsearch。对于需要良好可伸缩性和性能的云和分布式环境，Elasticsearch 是更好的选择。

- 两者都有良好的商业支持（咨询，生产支持，整合等）。

- 两者都有很好的操作工具，尽管 Elasticsearch 因其易于使用的 API 而更多地吸引了 DevOps 人群，因此可以围绕它创建一个更加生动的工具生态系统。

- Elasticsearch 在开源日志管理用例中占据主导地位，许多组织在 Elasticsearch 中索引它们的日志以使其可搜索。虽然 Solr 现在也可以用于此目的，但它只是错过了这一想法。

- Solr 仍然更加面向文本搜索。另一方面，Elasticsearch 通常用于过滤和分组，分析查询工作负载，而不一定是文本搜索。

- Elasticsearch 开发人员在 Lucene 和 Elasticsearch 级别上投入了大量精力使此类查询更高效(降低内存占用和 CPU 使用)。

- 因此，对于不仅需要进行文本搜索，而且需要复杂的搜索时间聚合的应用程序，Elasticsearch 是一个更好的选择。

- Elasticsearch 更容易上手，一个下载和一个命令就可以启动一切。Solr 传统上需要更多的工作和知识，但 Solr 最近在消除这一点上取得了巨大的进步，现在只需努力改变它的声誉。

- 在性能方面，它们大致相同。我说“大致”，因为没有人做过全面和无偏见的基准测试。对于 95％ 的用例，任何一种选择在性能方面都会很好，剩下的 5％ 需要用它们的特定数据和特定的访问模式来测试这两种解决方案。

- 从操作上讲，Elasticsearch 使用起来比较简单，它只有一个进程。Solr 在其类似 Elasticsearch 的完全分布式部署模式 SolrCloud 中依赖于 Apache ZooKeeper，ZooKeeper 是超级成熟，超级广泛使用等等，但它仍然是另一个活跃的部分。

- 也就是说，如果您使用的是 Hadoop，HBase，Spark，Kafka 或其他一些较新的分布式软件，您可能已经在组织的某个地方运行 ZooKeeper。

- 虽然 Elasticsearch 内置了类似 ZooKeeper 的组件 Xen，但 ZooKeeper 可以更好地防止有时在 Elasticsearch 集群中出现的可怕的裂脑问题。

- 公平地说，Elasticsearch 开发人员已经意识到这个问题，并致力于改进 Elasticsearch 的这个方面。

- 如果您喜欢监控和指标，那么使用 Elasticsearch，您将会进入天堂。这个东西比新年前夜在时代广场可以挤压的人有更多的指标！Solr 暴露了关键指标，但远不及 Elasticsearch 那么多。

  > 具体指标  http://solr-vs-elasticsearch.com/