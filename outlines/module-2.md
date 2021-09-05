---
description: >-
  This document outlines the contents and methodology of Module 2, focussed on
  machine-learning for record linkage.
---

# Machine learning

{% hint style="info" %}
This is a draft outline! Please feel free to [contact Miquel Duran-Frigola](mailto:miquel@ersilia.io) for suggestions or edits. A longer version of this page is available [here](https://docs.google.com/document/d/1oxoQqWTHVYk_A9E0tFHWZdqltlIQh2aX/edit).
{% endhint %}

**Facilitators:** Victor Olago \(VO\) and Miquel Duran-Frigola \(MDF\)

## Towards an end-to-end record linkage pipeline using machine learning

The aim of this course is to explore the potential of Machine Learning \(ML\) techniques applied to Record Linkage \(RL\). We will start the course by providing a gentle introduction to ML. Then, in a series of more specialized sessions, we will revisit the classical steps of record linkage \(data processing/cleaning, blocking, comparison...\) and will try to understand how ML can be used to increase linkage quality, performance and level of automation.

The course will be structured in 4 introductory sessions \(including real-life scenarios encountered by the facilitators\) and 2 hands-on sessions focused on synthetic datasets provided to participants.

## ML1. Demystifying machine learning for medical data analysis

<table>
  <thead>
    <tr>
      <th style="text-align:left">Session 2.1</th>
      <th style="text-align:left">General audience</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Content</td>
      <td style="text-align:left">
        <p>Past, present and future of ML applied to Medical Data Analysis. The field
          of ML is very broad; and an emphasis will be put on clarifying concepts
          and simplifying them for a general audience. Concepts include:</p>
        <ul>
          <li>A brief overview of the machine learning cycle
            <ul>
              <li>Data preparation</li>
              <li>Splitting data into train, test and validation sets</li>
              <li>Training a ML model</li>
              <li>A taxonomy of ML models, including the most prominent families of ML models</li>
              <li>Cross-validation and external validation</li>
              <li>Bringing models to production (model deployment)</li>
            </ul>
          </li>
          <li>Links between ML and conventional tools in statistics (the past)</li>
          <li>A selection of medical data analysis studies/articles applying ML (the
            present)</li>
          <li>End-to-end pipelines and the promises of ML; how the ML cycle will be
            embedded in medical data management centers (the future)</li>
        </ul>
        <p>Based on this general introduction, participants will be encouraged to
          suggest at least one current task in their own field of research where
          ML could be applied.
          <br />
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Learning outcomes</td>
      <td style="text-align:left">
        <p></p>
        <p>This session is aimed at a general audience and provides a high-level
          overview of ML. At the end of the session, attendants should have a &#x2018;demystified&#x2019;
          view of ML and, hopefully, they will be encouraged to explore the potential
          of ML in their own projects. Thus, the main outcomes are:</p>
        <ol>
          <li>A qualitative understanding of the field of ML</li>
          <li>A personalized list of items/tasks related to participant&#x2019;s projects
            where ML could be applied</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Format</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>Pre-recorded video (MDF)</li>
          <li>Forum: &#x201C;How can ML aid my data analysis pipelines&#x201D;?</li>
          <li>Extra materials
            <ol>
              <li>Selection of videos providing further insights into ML</li>
              <li>Selection of timely scientific articles applying ML to medical data analysis</li>
            </ol>
          </li>
          <li>Online Q&amp;A - VO and MDF will (1) summarize forum discussion and (2)
            answer participant&#x2019;s questions</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Duration</td>
      <td style="text-align:left">
        <ul>
          <li>45 min (video)</li>
          <li>Forum discussion (at least 30 min)</li>
          <li>Extra materials (optional)</li>
          <li>Online Q&amp;A (30 min)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Modality</td>
      <td style="text-align:left">Sync and Async</td>
    </tr>
    <tr>
      <td style="text-align:left">Prerequisites</td>
      <td style="text-align:left">None</td>
    </tr>
    <tr>
      <td style="text-align:left">Additional notes</td>
      <td style="text-align:left">This first session is not directly related to RL. In our opinion, it is
        important to provide a general overview of ML before exploring its applications
        to RL. Thus, we hope that this session will be interesting to a very broad
        audience, including participants not directly involved in data linkage
        studies.</td>
    </tr>
  </tbody>
</table>

## ML2. How can machine learning improve my record linkage procedures?

<table>
  <thead>
    <tr>
      <th style="text-align:left">Session 2.2</th>
      <th style="text-align:left">Partners ESTHER project, Epidemiology MSc/PhD students, Epidemiologists,
        Data managers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Content</td>
      <td style="text-align:left">
        <p>The classical record linkage pipeline will be revisited from the perspective
          of ML. In particular, we will explore how ML can:</p>
        <ul>
          <li>Aid data preprocessing by providing automated schema matching (detection
            of fields), correction of spelling errors, and abstract (embedded) representation
            of noisy entries.</li>
          <li>Speed up blocking/indexing based on vectorial representation of data and
            high-performance clustering and nearest neighbors searches.</li>
          <li>Refine identification of candidate linkage pairs based on multi-dimensional
            comparison vectors.</li>
        </ul>
        <p>We will put the emphasis on large-scale performance and application to
          low-resourced settings.</p>
        <p>In addition, we will distinguish between &#x2018;mature&#x2019; ML methods
          for RL and &#x2018;exploratory&#x2019; ones.</p>
        <p>To a lesser extent, we will discuss privacy-preserving ML methodologies
          and synthetic data generation, although these will not be the main focus
          of this session.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Learning outcomes</td>
      <td style="text-align:left">At the end of this session, participants will be able to identify the
        specific ML techniques that can be applied at each step of the RL pipeline.</td>
    </tr>
    <tr>
      <td style="text-align:left">Format</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>Pre-recorded video (MDF)</li>
          <li>Forum: &#x201C;A critical view on ML applied to RL. When is ML necessary
            and when it is not? What can we expect from it? (MDF &amp; VO)</li>
          <li>A minimal list of extra materials - participants will be encouraged to
            explore the literature on their own and share their findings (MDF &amp;
            VO)</li>
          <li>Online Q&amp;A (30 min) (MDF &amp; VO)</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Duration</td>
      <td style="text-align:left">
        <ul>
          <li>1h (video)</li>
          <li>Forum discussion (at least 1h)</li>
          <li>Extra materials (optional)</li>
          <li>Online Q&amp;A (30min)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Modality</td>
      <td style="text-align:left">Sync and Async</td>
    </tr>
    <tr>
      <td style="text-align:left">Prerequisites</td>
      <td style="text-align:left">ML1 &amp; Introduction to Probabilistic Record Linkage</td>
    </tr>
    <tr>
      <td style="text-align:left">Additional notes</td>
      <td style="text-align:left">This session underlines the interaction between ML and RL. No technical
        skills are required and therefore it will be aimed at a general audience.
        Discussion will be focused on developing a critical view on ML, so as to
        manage expectations and ultimately identify realistic applications of this
        family of techniques to RL.</td>
    </tr>
  </tbody>
</table>

## ML3. Case example 1: Unsupervised ML

<table>
  <thead>
    <tr>
      <th style="text-align:left">Session 2.3</th>
      <th style="text-align:left">Partners ESTHER project, Data managers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Content</td>
      <td style="text-align:left">In this session, we will introduce the taxonomy of unsupervised ML methods,
        with a focus on clustering algorithms. We will present a real-case scenario,
        based on a RL pipeline developed by VO at the NCR. Python code (but not
        data) will be fully or partially shared with participants through a GitHub
        repository for educational purposes.</td>
    </tr>
    <tr>
      <td style="text-align:left">Learning outcomes</td>
      <td style="text-align:left">At the end of this session, and by means of a real-world example relevant
        to the ESTHER project, participants will have a clear idea of the potential
        of unsupervised ML for RL, as well as the key requirements (both on terms
        of infrastructure and coding skills) that are needed to successfully develop
        a RL study.</td>
    </tr>
    <tr>
      <td style="text-align:left">Format</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>Pre-recorded video 1: A brief introduction to unsupervised ML methods
            (VO)</li>
          <li>Pre-recorded video 2: Introduction and results of a RL pipeline based
            on clustering, applied at NCR (VO)</li>
          <li>Webinar: Guided walk through code exposed in a GitHub repository (VO &amp;
            MDF)</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Duration</td>
      <td style="text-align:left">
        <ul>
          <li>20min (video 1)</li>
          <li>20min (video 2)</li>
          <li>30min (async code revision)</li>
          <li>1h (webinar)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Modality</td>
      <td style="text-align:left">Sync and Async</td>
    </tr>
    <tr>
      <td style="text-align:left">Prerequisites</td>
      <td style="text-align:left">ML2 and elementary coding skills. Ideally, knowledge of Python and familiarity
        with GitHub repositories.</td>
    </tr>
    <tr>
      <td style="text-align:left">Additional notes</td>
      <td style="text-align:left">This session will offer participants the opportunity to observe a real-case
        scenario for RL. Therefore, this is not yet a hands-on session per se.
        Hands-on sessions will be done in ML5 &amp; ML6. We&#x2019;d like to explore
        the idea of a tandem webinar where the narrative of the main facilitator
        (presenter) is complemented by comments from the assistant facilitator
        (chat).</td>
    </tr>
  </tbody>
</table>

## ML4. Case example 2: Supervised ML

<table>
  <thead>
    <tr>
      <th style="text-align:left">Session 2.4</th>
      <th style="text-align:left">Partners ESTHER project, Data managers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Content</td>
      <td style="text-align:left">In this session, we will introduce the taxonomy of supervised ML methods,
        with a focus on binary classification methods. Like in ML3, we will present
        a real-case scenario, this time based on an analysis of CIDRZ data. Different
        to ML3, focus will be put on three key steps (rather than the full pipeline),
        namely schema matching, full name sorting and comparison vector classification.
        Python code (but not data) will be fully shared with participants through
        the course GitHub repository.</td>
    </tr>
    <tr>
      <td style="text-align:left">Learning outcomes</td>
      <td style="text-align:left">It is impossible to cover in one session the plethora of supervised ML
        methods available today. Rather, participants will see in detail, and in
        a real case, how three supervised ML methods are applied to RL, including
        means to validate them.</td>
    </tr>
    <tr>
      <td style="text-align:left">Format</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>Pre-recorded video 1: A brief introduction to supervised ML methods (MDF)</li>
          <li>Pre-recorded video 2: Introduction and problems encountered in a record
            linkage study performed at CIDRZ (MDF)</li>
          <li>Webinar: Guided walk through code exposed in a GitHub repository (MDF
            &amp; VO)</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Duration</td>
      <td style="text-align:left">
        <ul>
          <li>20min (video 1)</li>
          <li>20min (video 2)</li>
          <li>30min (async code revision)</li>
          <li>1h (webinar)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Modality</td>
      <td style="text-align:left">Sync and Async</td>
    </tr>
    <tr>
      <td style="text-align:left">Prerequisites</td>
      <td style="text-align:left">ML2 and elementary coding skills. Assistance to ML3 highly recommended.
        Ideally, knowledge of Python and familiarity with GitHub repositories.</td>
    </tr>
    <tr>
      <td style="text-align:left">Additional notes</td>
      <td style="text-align:left">If deemed necessary, part of the time devoted to this session can be dedicated
        to (a) a general overview of Python ML packages or (b) the general functioning
        of version control repositories such as GitHub. Both elements are instrumental
        to data scientists today and we can decide whether these concepts shall
        be introduced in the course. As they are not directly related to RL, we
        may cover them indirectly or simply encourage participants to learn on
        their own.</td>
    </tr>
  </tbody>
</table>

## ML5. Hands-on 1: Design and development of an end-to-end ML/RL pipeline

<table>
  <thead>
    <tr>
      <th style="text-align:left">Session 2.5</th>
      <th style="text-align:left">Data managers, ESTHER partners</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Content</td>
      <td style="text-align:left">We will use a synthetic, small-scale dataset to develop an end-to-end
        ML-based pipeline for RL. The project will be developed collaboratively
        between all participants, including facilitators. In the first round of
        discussions, participants will be asked a series of questions regarding
        the project planning, including the choice of algorithms for each of the
        key steps. An end-to-end notebook for record linkage will be developed
        collaboratively. At the end of the hands-on session, participants will
        present to their supervisors (e.g. ESTHER partners).</td>
    </tr>
    <tr>
      <td style="text-align:left">Learning outcomes</td>
      <td style="text-align:left">Participants will experiment with ML tools in Python, including basic
        data analysis and plotting packages. In addition, they will develop a customized
        RL pipeline.</td>
    </tr>
    <tr>
      <td style="text-align:left">Format</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>Webinar: Design of the computational pipeline and distribution of tasks
            between participants</li>
          <li>Coding and issue tracking</li>
          <li>Short presentation of results</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Duration</td>
      <td style="text-align:left">
        <ul>
          <li>45min webinar</li>
          <li>3 days of coding (3h/day)</li>
          <li>30min presentation</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Modality</td>
      <td style="text-align:left">Sync and Async</td>
    </tr>
    <tr>
      <td style="text-align:left">Prerequisites</td>
      <td style="text-align:left">Python coding skills and familiarity with GitHub. Knowledge of Jupyter
        Notebooks is a plus. It is assumed that participants will know the synthetic
        dataset since it will be used in the probabilistic record linkage sessions.
        Likewise, it is assumed that the synthetic dataset will be available in
        a preprocessed form.</td>
    </tr>
    <tr>
      <td style="text-align:left">Additional notes</td>
      <td style="text-align:left">The necessary level of intervention by facilitators will largely depend
        on Python skills of participants. It is not possible to teach the Python
        programming language within the framework of this course. It would be advisable
        to distribute a survey before course commencement. Also, sessions ML3 &amp;
        ML4 will be useful to understand the level of Python proficiency of participants.</td>
    </tr>
  </tbody>
</table>

