---
layout: page
permalink: /teaching/
title: Teaching
description: 
nav: true
nav_order: 5
toc:
  sidebar: left
---

## Teaching Goals

As an instructor focused on biomedical engineering, my primary teaching goals are to provide students with skills applicable beyond the classroom, and to connect course content with the real-world applications through both lecture content and hands-on experiences. I feel comfortable teaching introductory courses on engineering, biomechanics, and programming in Python, MATLAB, or R, as well as intermediate or advanced engineering courses focused on biomechanics and programming for engineers. I am also comfortable teaching courses directly related to my research focus, particularly courses centered around current topics in neurotrauma and concussion research. 

## Real World Applications in the Classroom

I believe the best way to learn is by connecting classroom concepts to real-world applications. As an instructional teaching assistant, I have aimed to bring relevance to the classroom. In Fall 2023, as I approached the end of my dissertation work, I had the opportunity to serve as an instruction-focused TA for Fundamentals of Neurotrauma, contributing to lecture content, course syllabus, and assessments. As the course content of Fundamentals of Neurotrauma heavily overlapped with large portions of my research and findings, I actively incorporated this on-going research as I assisted in course development. For example, an early class lecture was heavily built around a conference presentation I was scheduled to give mid-semester. The lecture began with a continuation of a previous lecture and discussion on mechanisms to study head injuries, and transitioned into my lecture focusing on current research surrounding head impact exposure devices and the shortcomings in both device design and accepted testing methods.

I am currently designing additional assignments to allow students to work with real data I have collected, and to replicate my analysis and simulation methods. In general, I prefer to supplement lecture content with examples of practical applications. As an undergraduate, I found many of the course concepts in the biomedical engineering curriculum abstract and difficult to contextualize. As an instructor, I try to bring examples to the classroom where I can highlight a lesson and say “here is how I use this in my day-to-day work.”

## Practical Assessments

In a practical scenario, students have access to a variety of resources, ranging from textbooks and formula lists to reference books on material properties. Rather than require students to memorize easily referenced formulas, I find that allowing students access to these materials is more realistic. Instead of asking students to “solve for X,” I prefer to present information in a manner they may see it in the real world.  As a hypothetical example, for a course on intermediate biomechanics, an assessment of understanding of fracture tolerance, injury risk, and kinematics could be structured as a case report. Students can be presented with an autopsy report, injury risk curves, and a case scenario, and asked what events are most likely to have caused the observed injuries, and to justify using diagrams, calculations, and explanation as relevant. Rather than ask directly for the calculations, I present the information required to solve the problem, and allow the students to find the appropriate methods and develop a solution on their own.

As another example, I am currently developing an assignment for a course on Introduction to Neurotrauma. After teaching the class about finite element modeling, and specifically focusing on the SIMON head/brain injury model, students will be asked to determine whether or not certain head impacts are or are not injurious, based on field data on head movement from instrumented martial arts athletes. The students will be given raw data, and provided with the finite element model, and expected to determine whether the event was, or was not, potentially injurious. Rather than ask for specific injury metrics, I expect the students to take the information presented in class on a variety of calculated injury risk functions, and determine those for the events provided, as well as assess which are relevant to determine if the event caused an injury. Additionally, students will be expected to format the data and apply it appropriately to the model.

## Further Teaching Experience

As an undergraduate, I served as a TA for the introductory programming course for engineers, during a major transition from teaching MATLAB to teaching Python. As one of the few TAs for that course with extensive Python experience, I volunteered to organize and run review sessions for each exam. In my experience, it is most effective to learn to write code by actively writing code. With this in mind, I structured my review sessions as workshops, focusing on each concept individually, allowing students to work through sample problems, and then stepping through why various methods do or do not work. While I did not have access to the course feedback submitted by students, I noted a larger number of students at the second review session I held than were present at the first.



---


## Course Details

{% if site.data.courses.course_list %}
<article>
    <div class="cv">
      {% for entry in site.data.courses.course_list %}
        <a class="anchor" id="{{ entry.title }}"></a>
        <div class="card mt-3 p-3">
          <h3 class="card-title font-weight-medium">{{ entry.title }}</h3>
          {% if entry.department or entry.institution %}
            <table class="table-cv institution">
            <tbody>
              {% if entry.institution %}
              <tr>
                <td style="vertical-align: top; text-align: center;" class="institution"><i class="fas fa-university iconinstitution"></i></td>
                <td class="institution">{{entry.institution}}</td>
              </tr>
              {% endif %}
              {% if entry.department %}
              <tr>
                <td style="vertical-align: top; text-align: center;" class="department"><i class="far fa-dot-circle icondepartment"></i></td>
                <td class="department">{{entry.department}}</td>
              </tr>
              {% endif %}
            </tbody>
            </table>
            {% endif %}
          <div>
          {% include cv/time_table.html %}
          </div>
        </div>
      {% endfor %}
      </div>
  </article>
{% endif %}
