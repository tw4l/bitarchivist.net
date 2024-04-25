---
title: "Projects"
layout: page
path: "/projects"
---

## Personal Projects

### Brunnhilde

A Python command-line and GUI reporting tool for directories and disk images. Brunnhilde bundles tools such as [Siegfried](https://www.itforarchivists.com/siegfried), [ClamAV](https://www.clamav.net/), [bulk_extractor](https://forensicswiki.org/wiki/Bulk_extractor), The Sleuthkit (TSK)'s [tsk\_recover](https://sleuthkit.org/sleuthkit/man/tsk_recover.html), [HFS Explorer](http://www.catacombae.org/hfsexplorer/), and [fiwalk](https://www.forensicswiki.org/wiki/Fiwalk) to streamline appraisal and minimal processing of digital archives.

Brunnhilde was written to supplement existing file format identification and characterization tools, with a focus on producing human-readable high-level reports for digital archives and digital preservation practitioners. It is installed as a standard utility in the [BitCurator](https://wiki.bitcurator.net/index.php?title=BitCurator_Environment) environment.

**> Links:** [Github](https://github.com/tw4l/brunnhilde)

### Bulk Reviewer

Bulk Reviewer is an Electron desktop application that aids in identification, review, and removal of sensitive files in directories and disk images. Bulk Reviewer scans directories and disk images for personally identifiable information (PII) and other sensitive information using [bulk_extractor](https://github.com/simsong/bulk_extractor), a best-in-class digital forensics tool. The desktop application enables users to configure, start, and review scans; generate CSV reports of features found; and export sets of files (either those free of sensitive information, or those with PII that should be restricted or run though redaction software).

A previous server-based prototype developed during a summer fellowship at the [Harvard Library Innovation Lab](https://lil.law.harvard.edu/) using Django, Django REST Framework, and Vue.js can be found [here](https://github.com/tw4l/bulk-reviewer).

**> Links:** [Github](https://github.com/bulk-reviewer/bulk-reviewer), [Documentation](https://bulk-reviewer.readthedocs.io/en/latest/)

### METSFlask

A Flask web application for human-friendly exploration of Archivematica METS files.

**> Links:** [Github](https://github.com/tw4l/metsflask), [Live demo](http://bitarchivist.pythonanywhere.com)

### SCOPE

A digital archives access interface for Archivematica DIPs, built on Django and Elasticsearch, developed by Artefactual Systems and the Canadian Centre for Architecture.

I designed and developed the initial proof-of-concept prototype of SCOPE using Django between October 2017-May 2018, based on research conducted as CCA's first digital archivist from 2015 on.

**> Links:** [Github](https://github.com/cca-public/scope)

### CCA Tools (e.g. Disk Image Processor)

Digital archives processing tools intended for use in [BitCurator](https://wiki.bitcurator.net/index.php?title=BitCurator_Environment), an open source Ubuntu-derived Linux distribution for digital forensics and digital archiving.

**> Links:** [Github](https://github.com/cca-public/cca-tools)

### addext

Command-line Python utility to add file extensions to files without them, based on DROID/Siegfried PRONOM-based file format identification.

**> Links:** [Github](https://github.com/tw4l/addext)

### Independent Study: Access to Born-Digital Architectural Records (Spring 2015)

This independent study supplemented other coursework taken in the MS in Library and Information Science program at Simmons College. The study focused on preservation and access for digital architecture and design records such as computer aided design (CAD) and Building Information Modeling (BIM), and resulted in a 49-page paper on the subject entitled "Preservation and Access of Born-Digital Architectural Design Records in an OAIS-Type Archive."

**> Links:** [Reading list and paper](/projects/independentstudy/)

## Collaborative Open Source Projects I've Worked On

### Browsertrix

High fidelity cloud-native web archiving system implemented in Python/FastAPI (backend), Typescript/LitElement/Shoelace (frontend), and Kubernetes.

**> Links:** [Github](https://github.com/webrecorder/browsertrix), [Product site](https://browsertrix.com)

### Browsertrix Crawler

Web crawler implemented in TypeScript, Node.js, and Puppeteer, running in a single Docker container.

**> Links:** [Github](https://github.com/webrecorder/browsertrix-crawler)

### pwyb

Widely-used web archive discovery and playback system ("wayback machine") implemented in Python, JavaScript, and Vue.js.

**> Links:** [Github](https://github.com/webrecorder/pywb)

### Archivematica

Web-based digital preservation system to ingest, characterize, migrate, package, and store digital objects in accordance with the ISO-OAIS functional model, using archival standards such as METS, PREMIS, Dublin Core, and BagIt, implemented in Python, Django, and JavaScript.

**> Links:** [Github](https://github.com/artefactual/archivematica), [Documentation](https://archivematica.org/en/)

### Access To Memory (AtoM)

Web-based application for standards-based archival description and access in a multilingual, multi-repository environment, implemented in PHP and JavaScript.

**> Links:** [Github](https://github.com/artefactual/atom), [Documentation](**> Links:** [Github](https://github.com/artefactual/archivematica), [Documentation](https://archivematica.org/en/))
