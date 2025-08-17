Overview

Analyzes NYC Citibike usage to uncover demand patterns, rider behavior, and operational opportunities. The enhanced dashboard integrates temporal, spatial, and user-segment views for action-oriented insights.

Objectives

Ridership trends by hour, day, and season.
Station-level demand and imbalances (pickups vs. drop-offs).
Subscriber vs. casual behavior and trip durations.
Rebalancing signals and capacity planning.


Data Sources

Citibike trip data (public monthly CSVs): start/end stations, timestamps, user types, bike types.
Station metadata (location, capacity).
Weather (optional) for context.


Methodology

Ingest monthly CSVs; normalize time zones.
Clean data: remove duplicates, filter negative/implausible durations, handle missing stations.
Feature engineering: hour, weekday, season, trip distance proxies.
Aggregations: station net flows and time-bucket summaries.
Tableau visuals with filters and map layers.


Key Views and Interactions

Heatmap: rides by hour and weekday (commuter peaks).
Station map: bubble size by starts, color by net flow.
Duration distribution by user and bike type.
Monthly trends with optional weather overlays.

Findings and Insights

Strong weekday rush-hour peaks; weekend leisure spikes.
Transit-adjacent stations show marked morning pickups and evening returns.
Casual riders have longer median durations; e-bikes shorten trips but expand reach.
Seasonality drives higher ridership and broader utilization.


Limitations

Station relocations/closures complicate comparisons.
Weather granularity limits causal interpretation.
Data quality issues require continuous cleaning.
