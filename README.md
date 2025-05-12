# MCP Outlook Integration Fork

This repository was a fork of [kacase/mcp-outlook](https://github.com/kacase/mcp-outlook).

## Contribution

The primary contribution from this fork was the implementation of a feature to add attendees to existing calendar events. This functionality was merged into the upstream repository via [Pull Request #1](https://github.com/kacase/mcp-outlook/pull/1) 
[Commit](https://github.com/kacase/mcp-outlook/pull/1/commits/a91214804f52fe3c951f67ce2e6fae39433ea9b9).

Key enhancements included:
- Definition of new data structures (`AttendeeSchema`, `AddAttendeesToEventSchema`) in `src/types.ts`.
- Extension of `CalendarEventSchema` and `CreateEventSchema` in `src/types.ts` to optionally include attendees.
- Implementation of an `addAttendeesToEvent` method in `src/graphClient.ts` using a PATCH request to merge new attendees with existing ones.
- Introduction of a new MCP tool, `addAttendeesToCalendarEvent`, in `src/index.ts`.

## Archival

As the contributions have been successfully merged into the main `kacase/mcp-outlook` repository, this fork is now archived. Please refer to the original repository for the latest code, ongoing development:

[https://github.com/kacase/mcp-outlook](https://github.com/kacase/mcp-outlook)
