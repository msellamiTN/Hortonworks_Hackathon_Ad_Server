<h3>Hortonworks Hackathon - Ad Servering App</h3>
May 25, 2017
<br>
<br><b>Assets:</b>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;Presentation
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;One-Pager
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;NiFi Template (used for website orchestration, clickstream routing, enrichment)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;SAM Real-time Workflow (used for realtime analytics & machine learning, time windowing)
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;Spark / Zeppelin Notebook (used to build predictive models for campaign recommendations based on user demographics and historical clickstream data)
<br>
<br><b>HBase DDL:</b>
<br>Create ‘campaign’,’campaign_info’
<br>Create ‘company’,’company_info’
<br>Create ‘user’,’user_info’
<br>
<br><b>Schema Registry Record for "adserver":</b>
<br>{
 "type": "record",
 "namespace": "adserver",
 "name": "adserver",
 "fields": [
  {
   "name": "userid",
   "type": "string"
  },
  {
   "name": "campaignid",
   "type": "string"
  },
  {
   "name": "timestamp",
   "type": "string"
  },
  {
   "name": "mediatype",
   "type": "string"
  },
  {
   "name": "adtype",
   "type": "string"
  },
  {
   "name": "activity",
   "type": "string"
  },
  {
   "name": "city",
   "type": "string"
  },
  {
   "name": "state",
   "type": "string"
  },
  {
   "name": "age",
   "type": "int"
  },
  {
   "name": "campaign_area",
   "type": "string"
  },
  {
   "name": "campaign_category",
   "type": "string"
  }
 ]
}
<br>
<br><b>References:</b>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;<a href="https://hortonworks.com/products/data-center/hdp/">Hortonworks Data Platform (HDP)</a>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&bull;&nbsp;<a href="https://hortonworks.com/products/data-center/hdf/">Hortonworks Data Flow (HDF)</a>
<br>
<br><b>Screenshots:</b>
<br>
<br>Superset Realtime Dashboard (running on Apache Druid):
<br><img src="./screenshots/Screen Shot 2017-05-25 at 10.09.56 AM.png" class="inline"/>
<br>
<br>NiFi Flow - Orchestrates the Ad Server by accepting HTTP requests, processing data, and pushing clickstream data to Kafka for real-time analytics:
<br><img src="./screenshots/Screen Shot 2017-05-26 at 9.43.06 AM.png" class="inline"/>
<br>
<br>Website - Showing Ads based on real-time models, clickstream enrichment, and business rules:
<br><img src="./screenshots/Screen Shot 2017-05-25 at 10.10.38 AM.png" class="inline"/>
<br>
<br>Spark (Zeppelin Notebook) - Used to build predictive models to recommend relevant campaigns based on user demographics and historical clickstream data.
<br><img src="./screenshots/Screen Shot 2017-05-26 at 1.26.07 PM.png" class="inline"/>
<br>
