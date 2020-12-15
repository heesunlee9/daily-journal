# Master defense 

Title: DANIEL: Towards Automated Bug Discovery by Black Box Test Case 
Generation and Recommendation
Candidate: Michael Peechatt \
E-mail: mp6510@rit.edu \
Defence Date: Tue, 12/15/2020 \
Time: 1:00 pm \
Location: https://rit.zoom.us/j/96733799563 \
URL: https://gitlab.com/mp6510/daniel 


Abstract:Finding and documenting bugs in software is an essential component
of the development process. A bug is defined as a series of steps that
produces behavior which differs from the software specification and
requirements. Finding steps to produce such behavior requires expert
knowledge of the possible operations of the software in development, as well
as intuition and creativity. This thesis proposes DANIEL (Directed Action
Node Input Execution Language), a language that represents test cases as
directed graphs, where each node represents an action, and possible input
arguments for each action are represented along the incoming directed edges.
With this representation, it is possible to form a union of all recorded test
cases, making a combined directed graph which represents all the paths of
interaction with the developing software. This thesis demonstrates how DANIEL
can generate prioritized test cases for a web form application, while also
preserving workflow context. Using a graph G built on N = 500 Selenium test
cases, we evaluate a random walk, a weighted walk, and walks guided by
logistic regression and XGBoost models. We find the weighted walk discovers
the most bugs while the machine learning walk provides the most meaningful
coverage.


Chair: Alex Ororbia II \
Reader: Carlos Rivero \
Observer: Michael Mior

- meta bug \
- limitation : binary classification 이라는 거, changing label(결국 손 너무 많이 감) 

# feedback

이미지, “”, 인용표시 제대로 \
끝에 references 다는 걸로는 불충분 \

The thing you describe as “Active Leraning” I would call semi-supervised leraning? When did “Active Learning” become a term?? \
=> 용어 사용 주의. 정확한 용어. 이 학생은 

p(y, x) is usually the target for semi-supervised learning using a lot of x that only some have y whereas active learning is focused only supervised learning, but we want to expand the set of (x,y) with a model guiding the human to which samples to label

Unlabeled data 특징을 잘 이용 못하고 있다. 그냥 data 많이 넣기만 하고 있다. 


# My critique 
Q: dijkstra : "test cases cannot make sure there is no bug in software". When I use DANIEL, it is possible to prove it? 
A: No, it is undecidable. 
=> disclaimer needed. (이건 다루지 않는 다고)
=> 훌륭. 그러나 이거 보다 완성도 높혀야 한다. 조금 단순해 보이기는 했다. 딥러닝 부분이 적다. 딥러닝 말고 기초 통계기법으로 해봤으면 
=> mathmetical work, statistic work 가 더 있었으면 좋겠다. \
=> ML 을 x 에 어떻게 응용 할까? 
=> 새로운 언어를 만들었다는 거는 fantastic. 
=> selenium + DANIEL - 웹 행동 보고 test case 자동 생성 - 너무 단순한 app


# idea
scalability? - most students do not cover this issue. Because it is a student's research. 
a student's research - too simple application or sample. 
Proof of no bug for a safety critical systems such as nuclear power plants - undecidable 이라고 해서 무결함 증명을 안할 수는 없다. 

"I take the blame for that"


