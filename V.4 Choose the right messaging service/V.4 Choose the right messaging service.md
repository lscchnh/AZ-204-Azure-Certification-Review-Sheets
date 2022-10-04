V.4 Choose the right messaging service ![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.001.png)![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.002.png)

mercredi 5 janvier 2022  10:59 



||Description |When |Characteristics |
| :- | - | - | - |
|Event Grid |![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.003.png)|<p>- **For events** </p><p>- Simple event publish-subscribe infrastructure with trusted (e.g. your own web server)</p><p>` `publishers</p>|<p>- **64 ko max/event** </p><p>![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.004.png)</p><p>/!\ Data = ref (url ou id) towards true data </p>|
|Event hubs |![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.005.png)|<p>- **For events** </p><p>- You need to support authentication for a large number of publishers</p><p>. </p><p>- You must register an event stream in Data Lake or Blob storage. </p><p>- You need an aggregation or analysis of your event stream. </p><p>- You need reliable messaging or resiliency. </p><p>- You need high throughput & scalability </p>|<p>**Partitions**: Event hubs divides communications into</p><p>buffers in which default).  events are recorded (24h by</p><p>**Capture**: Event hubs can save or a blob  events to a data lake</p><p>**Authentication**: All publishers are authenticated in azure event hubs and receive a token</p><p>` `that allows</p><p>them to send an event. </p>|
|Storage Queue |![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.006.png)|<p>- **For messages** </p><p>- High demand for sending messages </p><p>- Single queue, no additional stuff </p><p>- Tracking the progress of the message in the queue </p>|<p>- Unlimited queue size </p><p>- Until 2000msg/sec </p><p>- 64 ko max/msg </p><p>- No fifo guaranteed </p>|
|||• Easier audit and logs ||
|Service bus queue |![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.007.png)|<p>- **For messages** </p><p>Compared to azure storage queues: </p><p>- Support for larger messages </p><p>- Supports multiple delivery methods </p><p>- Guarantees FIFO </p><p>- Transaction </p><p>- RBAC </p>|256 Kb/msg max Queue size < 80GB |
|Service bus topics |![](Aspose.Words.4285fe98-9927-4b48-a773-b67ac6632ff4.008.png)|<p>**For messages** </p><p>Compared to queue  </p><p>• If several receivers planned </p>|<p>Not supported in basic princing tier   </p><p>filtering (sql) possible via subscription                                           </p>|

