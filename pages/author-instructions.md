---
title: "Author instructions"
---

{% from "_macros.html" import button %}


# Author instructions

MIDL 2020 submissions follow two tracks: *full* and *short* papers. All accepted full papers will be published as a volume in the [Proceedings of Machine Learning Research](http://proceedings.mlr.press/). We will be using [openreview.net](https://openreview.net) as a submission and reviewing platform, with a two-week period for author rebuttal and discussion for full-paper submissions.
<!-- To submit a paper, authors need to have an updated OpenReview account. Visit [http://openreview.net/profile](http://openreview.net/profile) after logging in. -->

{{ button("OpenReview conference website", "https://openreview.net/group?id=MIDL.io/2020/Conference") }}

<!-- After the registration period is over the Submission button will be inactive. To upload your pdf, select your paper and press “Revision”. -->

**Inquiries to the program chairs can be addressed directly to [pcs@2020.midl.io](mailto:pcs@2020.midl.io).**


---


<h2 id="video_instructions">Video instructions</h2>

[% .deadlines %]
* **Deadline to submit the recording** 22 June 2020
[% / %]

MIDL 2020 being a fully virtual conference, we have opted for a format where each paper (full and short) will take the form of a pre-recorded video, which we will make available to conference attendees. We will further offer the possibility to discuss the papers and presentations in Q&A (“oral”) and interactive (“poster”) sessions during the originally scheduled conference dates. All videos will be uploaded on the [MIDL Youtube channel](https://www.youtube.com/channel/UCd87UPUTt-oqTeGi8fQw-_w).

We request authors to prepare and upload a video recording of their presentation, **with the file of the slides as well** (instructions on where to upload the files will be communicated in due time).
[% .deadlines %]
* **Full paper (“oral”)** 15-minute presentation video,
* **  ** the PDF file of the slides,
* **  ** and an optional 1-minute video teaser.
* **Full paper (“poster”)** 5-minute presentation video,
* **  ** the PDF file of the slides,
* **  ** and a 1-minute video “teaser”.
* **Short paper** 5-minute presentation video,
* **  ** the PDF file of the presentation (a maximum of 5 slides),
* **  ** and 1-minute video “teaser”.
[% / %]

While voice only over slides will be OK, it will be great to also have the presenter face embedded within the slides in the video. While we are unable to provide individualized technical support to help you create these videos, we provide some examples on how to record videos on the [help page](video-help.html). The final recording has to meet the following requirements:

* `16/9` aspect ratio
* Resolution at least `1920x1080p`
* `20 frame per second` or more
* Saved in `.mp4` format
* Audio channel in `mono or stereo` (no 5.1 or any creative setup)
* `Less than 1GB`
* Slides of the presentation should be in `.pdf`

Except for the above duration and format requirements, the form of the presentation is left free. However, please make sure the video includes the title of the paper, the authors’ names and affiliations, and a mention to MIDL 2020.

We hope to make MIDL 2020 a success, despite the difficult situation and the unusual conference format, and we thank you for your cooperation.

---

<!-- ## Camera ready instructions -->
<h2 id="camera_ready_instructions">Camera ready instructions</h2>

[% .deadlines %]
* **<s>Camera ready deadline</s>** <s>28 May 2020</s>
[% / %]

We encourage authors to take into account the reviewers concerns and apply appropriate changes to your submission to improve its quality. If you need to go over the suggested page limit, you may do so while still aiming for conciseness.

Please use the LaTeX style files provided at: [https://github.com/MIDL-Conference/MIDLLatexTemplate](https://github.com/MIDL-Conference/MIDLLatexTemplate) (`midl-fullpaper.tex` for full papers, `midl-shortpaper.tex` for short papers).

**The final paper in PDF** format has to be uploaded on OpenReview by May 28th, using the "Revision" button and the “PDF” field.

### Detailed instructions for Full Papers
<!-- **Applies only to full papers.** -->

Once your final material is prepared according to the detailed instructions below, please upload a single zip file containing all the items on OpenReview by May 28th. To do so, please **use the “Revision” button and the “Source Latex” field added to the revision form**.

After making sure that your project compiles correctly with the standard `pdflatex` compiler, please include all the
 following items in a single zip folder latex project:

1. The main LaTex file, which should be named `"surname20.tex"`, where "surname" is replaced with the primary author's surname. The number 20 represents a 2-digit representation of the year of publication. This naming convention is necessary as per the PMLR format.

2. The bibliography should be in a single `.bib` file and named `“surname20.bib”` with the same convention as above.

3. Within the “surname20.tex” tex file, the document class should be:
<pre><code>\documentclass{midl}</code></pre>

4. You should also set the following variables before the \title command:
<pre><code>\jmlryear{2020}
\jmlrworkshop{Full Paper -- MIDL 2020}</code></pre>

5. The bibliography should be included in the paper using the following command:
<pre><code>\bibliography{surname20}</code></pre>

6. Please do NOT use the `\begin{thebibliography}` environment.

7. **Do not** use any `\vskip` or any other format/spacing altering commands. They will be removed during compilation.

8. Include the main PDF and all the Figures in the zip folder

9. Fill out and sign the [PMLR Publication Agreement](http://proceedings.mlr.press/pmlr-license-agreement.pdf) and add it in PDF format to the zip folder as part of your latex project.


###  Detailed instructions for Short Papers

This year, all accepted short papers will be gathered in an arXiv compendium. In order for your short paper to be included, you will need to create an arXiv submission and provide us with your arXiv paper id once you have finished your camera-ready version **by May 28**.

1. Start your submission at: [https://arxiv.org/](https://arxiv.org/)

2. Your PDF must follow the same format of the camera-ready version used for OpenReview, above.

3. Do not forget to update your latex headers with:
<pre><code>\jmlrproceedings{MIDL 2020}{Medical Imaging with Deep Learning 2020}
\jmlrvolume{}
\jmlryear{}
\jmlrworkshop{MIDL 2020 -- Short Paper}
\editors{}</code></pre>

4. Your “Report Number” must have the following format when creating your arXiv submission:
<pre><code>MIDL/2020/ExtendedAbstract/XXX</code></pre>
where `XXX` is your paper ID used by OpenReview (**NOT the submission ID**). You can find it in the URL of your OpenReview submission:
<pre><code>https://openreview.net/forum?id=XXX</code></pre>

5. Once your arXiv submission is created, send the link to your arXiv paper to [pcs@2020.midl.io](mailto:pcs@2020.midl.io).

---

## Full papers

Full papers contain well-validated applications or methodological contributions of deep learning algorithms in medical imaging. There is no strict limit on paper length. However, we strongly recommend keeping full papers at 8 pages (excluding references and acknowledgements). An appendix section can be added if needed with additional details but must be compiled into a single PDF. The appropriateness of using pages over the recommended page length will be judged by reviewers. Full papers will go through a **double-blind** peer-reviewing process via OpenReview, with a two-week period for author rebuttal and discussion. All accepted papers will be presented as posters with a selection of these papers will also be invited for oral presentation.

[% .deadlines %]
* **<s>Full-paper registration deadline</s>** <s>24 January 2020, 23:59, [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Full-paper submission deadline</s>** <s>30 January 2020, 23:59, [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Full-paper registration open</s>** <s>1 January 2020, 23:59, [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Reviews made available to authors and rebuttal period</s>** <s>From March 20th to March 27th 2020</s>
* **<s>Author/reviewers open discussion period</s>** <s>From March 27th to April 3rd 2020</s>
* **<s>Full-paper decisions released to authors</s>** <s>April 10th 2020</s>
[% / %]


## Short papers

Short papers are up to 3 pages (excluding references and acknowledgements) and can, for example, focus on preliminary novel methodological ideas without extensive validation. We also specifically accept short papers of recently published or submitted journal contributions to give authors the opportunity to present their work and obtain feedback from the community. Selection of short papers is based on a light **double-blind** review process via OpenReview, without a rebuttal/discussion period. All accepted abstracts will be presented as posters at the conference.

[% .deadlines %]
* **<s>Short-paper registration deadline</s>** <s>24 January 2020, 23:59, [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Short-paper submission deadline</s>** <s>30 January 2020, 23:59, [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Short-paper registration open</s>** <s>1 January 2020, 23:59 [UTC -12](https://www.timeanddate.com/time/map/) ([AoE](https://en.wikipedia.org/wiki/Anywhere_on_Earth) timezone)</s>
* **<s>Short-paper decisions released to authors</s>** <s>April 10th 2020</s>
[% / %]

---

## Paper registration step (important)

To be able to upload the PDF of a paper (full and short) before January 30th, authors have to create a submission on openreview with title, abstract and author information by January 24th (paper registration deadline).


## Latex template

To prepare your submission to MIDL 2020 either as a full or short paper, please use the LaTeX style files provided at:
[https://github.com/MIDL-Conference/MIDLLatexTemplate](https://github.com/MIDL-Conference/MIDLLatexTemplate).

**Make sure that the submitted PDF is anonymous**. Only the final, accepted version should have author names.


## Dual submission policy
### Full papers

Submissions that are substantially similar to papers that have been previously published, or accepted for publication, or that are submitted in parallel to other conferences with proceedings or journals, are not allowed.

### Short papers

In addition to original work, authors can choose to submit a shortened version of a recently (within the year 2019 or 2020) published, or submitted, journal publication to foster dissemination of high-quality work. Submissions that are substantially similar to versions that have been accepted or submitted in parallel to other conferences with proceedings are not allowed.

In both cases, dual submission of your paper to a non-peer reviewed website like arXiv is allowed. Similarly, submissions that have been presented at non-archival workshops (i.e., venues that do not have publication proceedings or publish only a very short abstract) do not violate the policy.

The policy is enforced during the whole reviewing process period.


## Withdrawing policy and rejected papers
Authors have the right to withdraw papers from consideration at any time until the paper submission deadline.
After the submission deadline and during the paper review/rebuttal/discussion process, it will not be possible to withdraw a paper.
After the decisions are announced, it will be possible for authors to withdraw a rejected paper.
If an author withdraws the paper, it will be deleted from the OpenReview hosting site.

<!-- ## Discussion period

The discussion period is a time when reviewers, area chairs and authors can have an open discussion about the paper.
We encourage all participants to ..................... -->

---

## Reviewing process
1. Submissions can be made either as a full or short paper.
1. Submissions are uploaded on OpenReview. The official reviews will be private during the review period, and will become publicly visible only after the reviews become available to authors. Comments that are posted by reviewers will remain anonymous.
1. Public commenting (i.e. anybody who is logged in can post comments) becomes possible only after the decisions have been released reviews are made available to authors. The author of a public comment can decide to post anonymously or not. Login is required before posting any comment.
1. Submissions to MIDL will be **double-blind** (Reviewers cannot see author names when conducting reviews, and authors cannot see reviewer names).
1. Short-paper submissions will undergo a lighter review, and do not have a period for rebuttal and author discussion.
1. Reviews of full papers will be made available to authors on March 20th, and the authors have until March 27th to submit a rebuttal.
1. The period from March 27th  to April 3rd will be for open discussion between the authors and reviewers (full paper only), with the Area Chair guiding the discussion towards essential points.
1. During the rebuttal/discussion period, authors cannot update the pdf of a paper. To submit your rebuttal and/or answer specific comments by the reviewers, please use the “official comments” button in OpenReview.
1. On April 10th, authors will be notified about the acceptance or rejection of their paper (both full and short papers).
1. Once the process is complete and a final decision is reached, the authors can choose to delete rejected submissions from the OpenReview hosting site.
1. Papers that are not accepted will be considered non-archival, and may be submitted elsewhere at the discretion of the authors. We strongly encourage taking into account the reviewers comments before resubmitting. During submission, the authors will have the option to indicate whether to have their submissions, the reviews, and the comments to be deleted from the OpenReview site, in case their submission is rejected.
