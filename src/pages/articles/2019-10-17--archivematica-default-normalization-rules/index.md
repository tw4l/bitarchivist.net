---
title: Archivematica default normalization rules
date: "2019-10-17"
layout: post
draft: false
path: "/blog/2019-10-17-archivematica-default-normalization-rules/"
category: "Archivematica"
tags:
  - "Archivematica"
  - "Digital archives"
  - "Digital preservation"
  - "Format normalization"
description: "Response to Evelyn McLellan's question about Archivematica's default file format normalization rules on the Archivematica Google Group."
---

*This response is in response to [a thread on the Archivematica Google Group about Archivematica's default normalization rules](https://groups.google.com/forum/#!topic/archivematica/0FkZjEmChdE), started by Evelyn McLellan of Artefactual Systems. For some reason, Google kept marking my post as spam and deleting it, so I've copied the text of my response here.*

Hi Evelyn,

Thank you for raising this question. I'm looking forward to what will hopefully be an open and interesting discussion.

At Concordia University Library, we are making some changes to the default FPR to make them conform with our local file format policies. There are slight differences between the format policies we are implementing for Special Collections and for our research repository, but the common changes we are making include disabling normalization to ffv1 in mkv for H264-encoded mp4s and disabling normalization to tiff for png images. We have discussed potentially also disabling normalization to tiff for jpegs in the future, a move that I am personally inclined toward but we have not yet committed to. We've found [the Bentley Historical Library's look at their own FPR](http://archival-integration.blogspot.com/2016/10/customizing-archivematicas-format.html) really helpful in thinking through our own situation.

It's a bit difficult to discuss format normalization in a vacuum, as the risks are in some cases related to other digital preservation practices such as infrastructure for bit preservation. As one example, one of the reasons uncompressed and losslessly compressed formats are typically preferred to lossy formats is because the impact of a bit flip is much more pronounced in the latter. Yet in many institutions, a considerable amount of resources are spent ensuring that such bit flips are (1) unlikely to happen, and (2) detectable and correctable when they do. We store multiple copies of content, often on different media and services to increase their resiliency, use filesystems and hardware that integrate native checksumming and error correction, and/or calculate and periodically verify file checksums for fixity. I would guess that many Archivematica users fall into this camp (although given the availability of various hosted versions of Archivematica, maybe that's not a safe assumption?). In cases where an institution has invested so heavily in bit preservation, I don't personally find arguments around the potential damage of bit flips in lossy compressed, ubiquitous formats like jpeg and png very compelling.

Certainly, if that infrastructure is not available and an Archivematica user is creating an AIP to write to tape or a network share without regular fixity audits, normalizing to formats like tiff makes a lot more impact. And as you point out in your post, there are other valid reasons for extensive normalization. But it also always comes at a cost, and some of the benefits (e.g. file validation) may be possible via other means.

As my co-authors and I argue in [a recent paper on environmental sustainability and digital preservation](https://doi.org/10.17723/0360-9081-82.1.165) ([OA copy via Harvard DASH](https://dash.harvard.edu/handle/1/40741399)), it's also worth considering whether format migrations need to happen at the moment of ingest or whether migration at the time of access/use might suffice for some use cases. Widely used FOSS migration tools used by Archivematica such as ImageMagick and ffmpeg are not likely to become unavailable any time soon, meaning that we may be able to responsibly defer some migration in the interests of not increasing the environmental footprint of our activities (keeping in mind that all of those bit preservation activities mentioned above tend to act as multipliers on our storage and energy footprints). The particular value and local context of collections may also mean that these trade-offs are worth it for some collections or content and not others, particularly when curators and preservationists employ tiered digital preservation models (as many of us do in practice, whether formally or just to maximize the impact of our resources).

I don't know that there are easy answers here for the default rules. I wonder if it might be useful to have a few easily selectable FPR "profiles" available to users. I can imagine a future where users are asked on setup to select how conservative they want to be with formats generally (say "Normalize everything possible" vs "Do not normalize ubiquitous formats"), and based on that selection the individual FPR rules for common formats like jpeg, png, H264 mp4 are enabled/disabled accordingly in one action.

Looking forward to hearing how others are thinking through these issues, and thanks again Evelyn for starting the discussion!
