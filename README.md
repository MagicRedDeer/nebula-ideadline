> Mirror of [nebulapipeline/nebula-ideadline](https://bitbucket.org/nebulapipeline/nebula-ideadline),
> part of the Nebula Pipeline. Kept here for reference; the original is canonical.

# nebula-ideadline

Deadline render-farm integration for the Nebula Pipeline, written against Deadline 10 and Maya.

- `deadlineWrapper.py` — a thin, typed layer over `DeadlineCommand`. Job submission, repository
  discovery and switching, pool and job queries, and `DeadlineJob` / `DeadlinePluginInfo` objects
  instead of shelling out to the CLI and parsing text at every call site.
- `maya/_deadlinemaya.py` — the Maya submitter. Builds a job from the current scene: render layers,
  cameras, frame ranges, output paths and the department's job metadata, then hands it to the wrapper.

This is Python 2 and pymel-era code, kept as it was written. It is an archive, not a maintained
package.

Architecture context for the modules either side of this one is in the
[Nebula Pipeline index](https://github.com/MagicRedDeer/nebula-pipeline).

LICENSE
=======

Copyright 2021. Talha Ahmed. All rights reserved.

This work is licensed under the terms of Eclipse Public License - v 2.0.
For a copy see https://www.eclipse.org/org/documents/epl-2.0/EPL-2.0.txt
