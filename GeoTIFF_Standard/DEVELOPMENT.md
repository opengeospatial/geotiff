## Development Guidelines

This document establishes guidelines which build a transparent,
open mechanism for managing development of the OGC GeoTIFF standard.
The GeoTIFF Standards Working Group (SWG) will follow these processes when creating version 1.0 of the standard.
Development of future versions may require modifications to these guidelines.
In that case, this document will be adjusted as necessary.
Modifications to this document are subject to the same process as modifications to the GeoTIFF standard.

## Driving factors

Version 1.0 of the OGC GeoTIFF standard strives to be an accurate rendition of the existing GeoTIFF 1.0 specification available from [https://trac.osgeo.org/geotiff](https://trac.osgeo.org/geotiff/).
Some divergence may be necessary where the original specification is no longer implementable.

## Specification Change Criteria

The specification *will evolve over time*.
Changes  may be made when any of the following criteria are met:

* Clarity. The current "way" something is done doesn't make sense, is complicated, or not clear.

* Consistency. A portion of the specification is not consistent with the rest, or with the industry standard terminology.

* Additional features. Version 1.0 reflects state of the art as of 1995. Additional features may be added to bring the standard up to the current state of the art.

## Specification Change Process

For each change in the specification we should *always* consider the following:

* Migration. Is this a construct that has a path from the existing 2.0 specification? If so, how complicated is it to migrate to the proposed change?

* Tooling. Strive to support code generation, software interfaces, spec generation techniques, as well as other utilities. Some features may be impossible to support in different frameworks/languages. These should be documented and considered during the change approval process.

* Visualization. Can the specification change be graphically visualized somehow in a UI or other interface?

Changes to the standard shall be approved by a majority of the SWG members.
Approval can be given by commenting on the issue itself, for example, "Approved by @mmouse".
After voting criteria is met, the PR will be merged by the editor.
No change should be approved unless it is documentation in an accompanying issue, branch, and PR.

## Tracking Process

GitHub is the medium of record for all spec designs, issues, and decisions.

The **human readable** document is the source of truth.
The documentation will live in a *.pdf file located in the root of the GeoTIFF GitHub project.

The GitHub repository contains three types of branches:

* master - Current stable version. No PRs would be accepted directly to modify the specification. PRs against supporting files can be accepted.

* v.<major>.<minor>.<corrigendum> - A working branch for developing the next version of the standard.

* <any> - A working branch used to capture changes related to a specific issue. These branches are used to create pull requests updating the next version branch. These branches should be associated with one or more issues which document the issues, discussions, and decisions driving these modifications to the standard.

Labels will be used to indicate the state of an issue or pull request.
Preliminary labels are:

* New - indicates a new issue or branch
* Bug - indicates an error in the standard
* Housekeeping - administrative issues
* Review - open for review and discussion
* Consensus - consensus has been achieved on an issue
* Rejected - no futher work will be performed
* Needs Approval - ready to be merged into the baseline

Additional labels may be created as needed.

An issue will be opened for each potential change to the standard.
The initial issue should include a clear and complete description of the problem to be addressed.
Discussion of how to address the problem should be conducted exclusively through the GitHub issue.
Once consensus has been reached, that consensus will be captured in the Issue.

If the consensus solution to an issue involves a change to the Standard,
then a Pull Request will be used to describe the *proposed* solution and linked to the original issue.
The Pull Request will be tagged with the "needs approval" label.

Pull Requests will be available for review and comment for two weeks.
If there are no unresolved objections, then the PR may be merged into the current baseline.

A PR may have conflicts which prevent its merger into the baseline.
In that case, the editor may divide the PR into multiple PRs to work around the issues.

