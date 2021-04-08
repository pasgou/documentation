=======
Surveys
=======

**Odoo Surveys** helps users create surveys, appraisals, quizzes, and questionnaires to gather
valuable information from their customers and/or employees.

Question configuration
======================

**Odoo Surveys** makes it easy for anyone to create compelling questions with just a couple clicks.
Choose from a wide array of *Question Types*, each with their own array of customizable features and
options.

Add a question
~~~~~~~~~~~~~~

When you click *Add a question* in the *Questions* tab on the survey template page, a pop-up
appears, in which you create your question.

After the question has been written in the *Question* field, you choose the *Question Type.* A
preview of the question type is shown in this window, as well.

.. image:: survey/preview-question-type.png
   :align: center
   :alt: Selecting a question type in Odoo Surveys

Answers and Options tab
~~~~~~~~~~~~~~~~~~~~~~~

Features change in the *Answers* and *Options* tab depending on the chosen *Question Type*. However,
there are some options that are available for all (or most) *Question Types*.

Such as *Validate Entry*, *Mandatory Answer*, *Question Time Limit* (for *Live Sessions*),
*Conditional Display*, and *Score*/*Scored*.

Validate Entry
**************

In the *Answers* tab (for most *Question Types*), there is an option to *Validate Entry*.

This allows users to choose a minimum and maximum response (e.g text length, date, etc.). You can
also customize the error message that appears beneath the field on the survey if an invalid answer
is entered.

Question Time Limit (for *Live Sessions*)
*****************************************

Timed questions are only available during *Live Session* surveys.

To put a time limit on a specific question, select the question you wish to modify, and go to
:menuselection:`Options Tab --> Question Time Limit`. At that point, you can specify the time
limit (in seconds).

.. image:: survey/question-time-limit.png
   :align: center
   :alt: Survey question time limit

Conditional Display
*******************

*Conditional Display* means a question is only displayed if the specified conditional answer has
been selected in a previous question.

After activating *Conditional Display*, you need to choose a *Triggering Question*. Once done, you
should select the *Triggering Answer* linked to that question.

.. image:: survey/conditional-triggering-answers.png
   :align: center
   :alt: Conditional triggering answer fields

To create a triggering question, you must save the question and the entire survey first. Then,
re-enter *Edit* mode, open the question template of the question you wish to modify, and open the
*Options* tab. Tick *Conditional Display* and proceed to select which question and answer will
trigger this particular question.

.. note::
   Triggering questions can only be multiple choice.

Score/Scored
************

This feature is only available in the *Answers* tab for the following *Question Types*: *Numerical
Value*, *Date*, and *Datetime*.

If the *Scored* box is ticked, that means this question will be scored, and you can determine
the exact *Score* in the field below. Then, when a participant enters the correct answer (also
indicated in the *Answers* tab of these *Question Types*), they will be rewarded with that
predetermined *Score*.

Question types and features
~~~~~~~~~~~~~~~~~~~~~~~~~~~

The following is a list of the available *Question Types* and their specific features:

* **Multiple Lines Text Box** - open-text field suitable for long answers where any type of text
  is allowed

  **Features**: *Mandatory answer*, *Question Time Limit* (for *Live Sessions*), and *Conditional
  Display*

* **Single Line Text Box** - open-text field suitable for short answers where any type of text is
  allowed

  **Features**: Force participants to enter an email address by ticking *Input must be an email*.
  Tick *Save as user nickname* to save their response as their username. Choose *Validate Entry*
  to configure a min/max text length

* **Numerical Value** - open-text field that only accepts a number as an answer

  **Features**: *Validate entry* (min/max number), *Correct answer* (numerical value),
  *Scored*/*Score*

* **Date** - date selection on a calendar

  **Features**: *Validate entry* (min/max date), *Correct answer* (date), and *Scored*/*Score*

* **Datetime** - date and time selection on a calendar

  **Features**: *Validate entry* (min/max date and time), *Correct answer* (date and time),
  and *Scored*/*Score*

* **Multiple choice: only one answer** - closed question where only one answer can be selected

  **Features**: *Choices* and the user selects one option

* **Multiple choice: multiple answers allowed** - closed question where multiple answers can be
  selected

  **Features**: *Choices* but the user can select more than one option

* **Matrix** - table of multiple choice questions that share the same possible answers

  **Features**: *Choices* and *Rows*, wherein the *Rows* represent a certain question and the
  *Choices* represent various answer options to that question

Survey options
==============

Customize and configure your survey in a number of different ways in the *Options* tab, located on
the survey template page.

The *Options* tab is split into 4 feature categories:

- *Questions*
- *Scoring*
- *Candidates*
- *Live Session*

Questions
~~~~~~~~~

This section primarily focuses on the overall presentation and layout of your survey. There are
also options featuring timed and randomized surveys.

First, you select the layout. You can choose from:

* *One page with all the questions*
* *One page per section*
* *One page per question*

You can also choose how you want to display the participant's progress during the survey. It can
either be shown as a *Percentage* or a *Number* (i.e. 1 of 20 answered).

Below that, you can decide if you'd like to present your participants with a *Back Button* during
the survey. You can also decide to modify the question selection to include all answers or have
them randomized by section. You can even add a time limit, as well.

.. image:: survey/questions-setting-section.png
   :align: center
   :alt: Questions section of survey settings

Timed surveys
*************

With timed surveys, participants must complete the survey within a predetermined amount of time.
You can apply the same time limit feature to individual questions, as well.

Timed surveys and questions ensure that all participants get the same amount of time to answer and
complete the survey. They also discourage participants from looking up answers with external
sources.

To set a time limit on a survey, select *Survey Time Limit* under the *Options* tab of your
survey, and enter the desired time limit (in minutes).

.. image:: survey/options-tab-time-limit.png
   :align: center
   :alt: View of a survey form emphasizing the time limit feature in Odoo Surveys

Before participants begin, they see how much allotted time they have to complete the survey. During
the survey, a timer is shown on the pages so the user can keep track of the remaining time.

.. image:: survey/time-limit-survey-clock.png
   :align: center
   :alt: Survey time limit clock display front-end

.. note::
   Surveys that are not submitted in time **do not** have their answers saved.

Randomized surveys
******************

When a survey is randomized, the questions will be shuffled in a random order every time a
participant opens the survey. Random surveys are a great way to eliminate the possibility of
participants copying off one another.

Once you've enabled that feature, go to the *Questions* tab of the survey, where a
*Random questions count* column is now present.

Here you can decide how many of the questions should be taken into account during the shuffling,
by simply selecting the number and changing it. That number corresponds to how many questions in
that section will be randomized.

.. image:: survey/random-questions-count.png
   :align: center
   :alt: Survey random questions count

Scoring
~~~~~~~

Surveys are a great way to measure a person's performance, knowledge of a subject, or overall
satisfaction.

Odoo allows you to attach points to certain answers of survey questions. These points are then
summed up to give your participant a final score.

Users have the option to choose between: *Scoring with answers at the end* **or** *Scoring without
answers at the end*.

If you select either *Scoring with answers at the end* or *Scoring without answers at the end*, two
more fields appear. In which, you decide what the *Success %* is, and you can choose to make this a
certification.

.. image:: survey/survey-options-scoring.png
   :align: center
   :alt: Survey option template tab

You can set the *Success %* here, as well. The *Success %* is the score the user will need to
achieve in order to have successfully taken the survey.

.. image:: survey/survey-success-percentage.png
   :align: center
   :alt: Survey success percentage setting

If *Is a Certification* is selected, you can choose its template. The certification is automatically
emailed to users who have successfully finished the survey.

.. image:: survey/survey-certification-template-setting.png
   :align: center
   :alt: Survey certification template setting

And, if you check the box next to *Give Badge,* you are able to select which Certification Badge
you want to give to your participants.

.. image:: survey/survey-scoring-section.png
   :align: center
   :alt: Scoring section of survey settings

.. note::
   The *Give Badge* feature is **only** available if you enable *Login required* in the
   *Candidates* section of the *Options* tab of the survey detail form.

Following those configurations, you can choose a survey question that you want to assign a point
value to, and mark which answer is "correct" on the question pop-up. You can also apply negative
point results for "incorrect" answers, as well.

.. image:: survey/answers-questions-points.png
   :align: center
   :alt: Answer tab of survey with questions and points

Candidates
~~~~~~~~~~

In this section, you can decide who can access this survey.

The *Access Mode* allows you to choose between *Anyone with the link* and *Invited people only*.
You can also decide if you want to grant access to *Appraisal Managers Only*. This person is the
one who manages the various appraisals/surveys.

You can also require participants to log in to access the survey.

You can limit the number of login attempts by ticking *Attempts Limit* and entering a number.

.. image:: survey/candidates-section.png
   :align: center
   :alt: Candidates section of survey settings

Live Session
~~~~~~~~~~~~

This section is dedicated to users who are conducting Live Session surveys, wherein they directly
engage with an audience at the same time - much like a live event.

Here, you can choose to reward participants with more points for quick answers. So, if more than
one participant were to choose the correct answer, the quickest (correct) response would be more
valuable, and thus given more points.

You can also customize the specific *Session Code* that participants would need in order to access
the Live Session survey here, as well.

.. image:: survey/live-session-setting.png
   :align: center
   :alt: Live session section of survey features

