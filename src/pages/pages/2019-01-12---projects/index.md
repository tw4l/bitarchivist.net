---
title: "Projects"
layout: page
path: "/projects"
---

### Brunnhilde

A Python command-line and GUI reporting tool for directories and disk images. Brunnhilde bundles tools such as [Siegfried](https://www.itforarchivists.com/siegfried), [ClamAV](https://www.clamav.net/), [bulk_extractor](https://forensicswiki.org/wiki/Bulk_extractor), The Sleuthkit (TSK)'s [tsk\_recover](https://sleuthkit.org/sleuthkit/man/tsk_recover.html), [HFS Explorer](http://www.catacombae.org/hfsexplorer/), and [fiwalk](https://www.forensicswiki.org/wiki/Fiwalk) to streamline appraisal and minimal processing of digital archives.

Brunnhilde is installed as a standard utiltity in the [BitCurator]((https://wiki.bitcurator.net/index.php?title=BitCurator_Environment)) environment.

[Github](https://github.com/timothyryanwalsh/brunnhilde)

### Bulk Reviewer

Bulk Reviewer is a software program that aids in identification, review, and removal of sensitive files in directories and disk images. Bulk Reviewer scans directories and disk images for personally identifiable information (PII) and other sensitive information using [bulk_extractor](https://github.com/simsong/bulk_extractor), a best-in-class digital forensics tool, and can optionally extract named entities (personal names as well as nationalities, religions, and political affiliations) using [spaCy](https://spacy.io/) and [Apache Tika](https://tika.apache.org/). A browser application enables users to configure, start, and review scans, generate reports, and export files, separating problematic files (e.g., those requiring redaction or further review) from those that are free of sensitive information.

Bulk Reviewer consists of two separate applications that communicate via websockets and a REST API:

* A backend application `server` built using [Django](https://www.djangoproject.com/), [Django Rest Framework](http://www.django-rest-framework.org/), [Celery](http://www.celeryproject.org/), [Django Channels](https://channels.readthedocs.io/en/latest/), [Postgres](https://www.postgresql.org/), [Redis](https://redis.io/) and [RabbitMQ](https://en.wikipedia.org/wiki/RabbitMQ).
* A frontend single page application (SPA) `client` built using [Vue.js](https://vuejs.org/).

[Github](https://github.com/timothyryanwalsh/bulk-reviewer)

### METSFlask

A Flask web application for human-friendly exploration of Archivematica METS files.

[Github](https://github.com/timothyryanwalsh/bulk-reviewer)

[Live demo](https://bitarchivist.pythonanywhere.com)

### CCA Tools (e.g. Disk Image Processor)

Digital archives processing tools intended for use in [BitCurator](https://wiki.bitcurator.net/index.php?title=BitCurator_Environment), an open source Ubuntu-derived digital forensics environment for digital forensics and digital archiving.

[Github](https://github.com/cca-public/cca-tools)

### addext

Command-line Python utility to add file extensions to files without them, based on DROID/Siegfried PRONOM-based file format identification.

[Github](https://github.com/timothyryanwalsh/addext)

### Independent Study: Access to Born-Digital Architectural Records (Spring 2015)

This independent study supplemented other coursework taken in the MS in Library and Information Science program at Simmons College. The study focused on preservation and access for digital architecture and design records such as computer aided design (CAD) and Building Information Modeling (BIM), and resulted in a 49-page paper on the subject entitled "Preservation and Access of Born-Digital Architectural Design Records in an OAIS-Type Archive."

[Reading list and paper](/projects/independentstudy/)