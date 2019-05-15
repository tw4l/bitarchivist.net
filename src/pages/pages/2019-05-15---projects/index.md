---
title: "Projects"
layout: page
path: "/projects"
---

### Brunnhilde

A Python command-line and GUI reporting tool for directories and disk images. Brunnhilde bundles tools such as [Siegfried](https://www.itforarchivists.com/siegfried), [ClamAV](https://www.clamav.net/), [bulk_extractor](https://forensicswiki.org/wiki/Bulk_extractor), The Sleuthkit (TSK)'s [tsk\_recover](https://sleuthkit.org/sleuthkit/man/tsk_recover.html), [HFS Explorer](http://www.catacombae.org/hfsexplorer/), and [fiwalk](https://www.forensicswiki.org/wiki/Fiwalk) to streamline appraisal and minimal processing of digital archives.

Brunnhilde was written to supplement existing file format identification and characterization tools, with a focus on producing human-readable high-level reports for digital archives and digital preservation practitioners. It is installed as a standard utility in the [BitCurator](https://wiki.bitcurator.net/index.php?title=BitCurator_Environment) environment.

**> Links:** [Github](https://github.com/timothyryanwalsh/brunnhilde)

### Bulk Reviewer

Bulk Reviewer is an Electron desktop application that aids in identification, review, and removal of sensitive files in directories and disk images. Bulk Reviewer scans directories and disk images for personally identifiable information (PII) and other sensitive information using [bulk_extractor](https://github.com/simsong/bulk_extractor), a best-in-class digital forensics tool. The desktop application enables users to configure, start, and review scans; generate CSV reports of features found; and export sets of files (either those free of sensitive information, or those with PII that should be restricted or run though redaction software).

A previous server-based prototype developed during a summer fellowship at the [Harvard Library Innovation Lab](https://lil.law.harvard.edu/) using Django, Django REST Framework, and Vue.js can be found [here](https://github.com/timothyryanwalsh/bulk-reviewer).

**> Links:** [Github](https://github.com/bulk-reviewer/bulk-reviewer)

### METSFlask

A Flask web application for human-friendly exploration of Archivematica METS files.

**> Links:** [Github](https://github.com/timothyryanwalsh/metsflask), [Live demo](http://bitarchivist.pythonanywhere.com)

### CCA Tools (e.g. Disk Image Processor)

Digital archives processing tools intended for use in [BitCurator](https://wiki.bitcurator.net/index.php?title=BitCurator_Environment), an open source Ubuntu-derived digital forensics environment for digital forensics and digital archiving.

**> Links:** [Github](https://github.com/cca-public/cca-tools)

### addext

Command-line Python utility to add file extensions to files without them, based on DROID/Siegfried PRONOM-based file format identification.

**> Links:** [Github](https://github.com/timothyryanwalsh/addext)

### Independent Study: Access to Born-Digital Architectural Records (Spring 2015)

This independent study supplemented other coursework taken in the MS in Library and Information Science program at Simmons College. The study focused on preservation and access for digital architecture and design records such as computer aided design (CAD) and Building Information Modeling (BIM), and resulted in a 49-page paper on the subject entitled "Preservation and Access of Born-Digital Architectural Design Records in an OAIS-Type Archive."

**> Links:** [Reading list and paper](/projects/independentstudy/)
