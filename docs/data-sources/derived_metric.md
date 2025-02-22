---
layout: "wavefront"
page_title: "Wavefront: Derived Metric"
description: |-
    Get the information about a certain Wavefront derived metric by its ID.
---

# Data Source: wavefront_derived_metrics

Use this data source to get information about a certain Wavefront derived metric by its ID.

## Argument Reference
* `id` - (Required) The ID associated with the derived metric data to be fetched.

## Example Usage

```hcl
#Get the information about a derived metric.
data "wavefront_derived_metric" "example" {
  id = "derived_metric_id"
}
```

## Attribute Reference

* `name` - The name of the derived metric in Wavefront.
* `id` - The ID of the derived metric in Wavefront.
* `query`- A Wavefront query that is evaluated at regular intervals (default is 1 minute).
* `minutes` - How frequently the query generating the derived metric is run.
* `in_trash` - A Boolean variable indicating trash status.
* `tags` - A set of tags assigned to the derived metric.
* `query_failing` - A Boolean variable indicating whether query is failing for the derived metric.
* `last_error_message` - Last error message occurred.
* `last_failed_time` - Timestamp of the last failed derived metric.
* `additional_information` - User-supplied additional explanatory information about the derived metric.
* `create_user_id` - The ID of the user who created the derived metric.
* `update_user_id` - The ID of the user who updated the derived metric.
* `status` - The status of the derived metric.
* `hosts_used` - A list of hosts used in the derived metric.
* `last_processed_millis` - The last processed timestamp.
* `process_rate_minutes` -  The specified query is executed every `process_rate_minutes` minutes.
* `points_scanned_at_last_query` - The number of points scanned when last query was executed.
* `include_obsolete_metrics` -A Boolean flag indicating whether to include obsolete metrics or not.
* `last_query_time` - The timestamp indicating the last time the query was executed.
* `metrics_used` - A list of metrics used in the derived metric.
* `query_qb_enabled` - A Boolean flag for enabling `query_qb`
* `deleted` - A Boolean flag indicating whether the derived metric is deleted or not.
* `created_epoch_millis` - The timestamp in epoch milliseconds indicating when the derived metric is created.
* `updated_epoch_millis` - The timestamp in epoch milliseconds indicating when the derived metric is updated.


	
