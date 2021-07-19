# Windows Pack
----
This pack is targeted for collections of Window events in the Classic or newer XML format. For events in the Classic format, sometimes the Message field contains XML.  These Message fields are also taken into consideration.  The `WindowsClassicEvents` and `WindowsXMLEvents` pipelines inside the pack gives you the ability to shape events into JSON or Key=Value format and dramatically reduce event sizes.

# Important Information
---
```
This pack may be incompatible with some Splunk dashboards that depend on specific field extractions.
Please review various Splunk add-ons and configuration files such as props.conf or transforms.conf and make adjustments as necessary.
```

# What to Expect
---
* Classic Event Reduction:  Expect up to 70% reduction in the event size.
* XML Event Reduction:  Expect a range from 25%-50% reduction in the event size.

## Requirements
---
Before you begin, ensure that you have met the following requirements:

1. Create a Route with with a filter for your Windows events
2. Select the `Windows` pack as the pipeline.

## Installation
---
Download the most recent .crbl file in the repo [`releases page`](https://github.com/criblpacks/cribl-windows-events/releases)

## Release Notes
---
### Version 0.5.3 - 2021-07-19
- Removed unnecessary Parser function at the end of the WindowsXML pipeline as this step contradicts the Eval functions above

### Version 0.5.2 - 2021-07-16
- Updated the README with additional release notes

### Version 0.5.1 - 2021-07-13
- Updated README with information for installing the pack
- Added actions for publishing .crbl from repo when new release is cut

### Version 0.5.0 - 2021-07-10
Initial release! Windows events are big and ugly and LogStream Packs are beautiful!

Support for: WindowsXMLEvents and WindowsClassicEvents


## Contributing to the Pack
---
Discuss this pack on our Community Slack channel [#packs](https://cribl-community.slack.com/archives/C021UP7ETM3).

## Contact
---
The author of this pack is David Maislin and can be contacted at <david@cribl.io>.

## License
---
This Pack uses the following license: [`Apache 2.0`](https://github.com/criblio/appscope/blob/master/LICENSE).
