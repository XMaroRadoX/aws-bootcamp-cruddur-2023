# π» Week 0 β Billing and Architecture π‘

## π°οΈ Learning Time
### ποΈ C4 Model

>I am watching the C4 Model video (https://youtu.be/x2-rSnhpw0g)

π Notes about it:

* Nobody likes UML (Unified language model) and rarely it is used, especially when the team is moving fast because it is not familiar to many people and has differences among them. π
* Communication is essential when doing team projects. Different people need to be presented with the information about the architecture according to their understanding. π¬
* C4 stands for Context, Containers, Components, and Code. It gives a map-like view of the structure, going from context -> containers -> components -> code. Going more to the right means you are viewing a more detailed view. πΊοΈ
* System context: shows how people and software interact with each other without mentioning details. It gives a good overview for non-technical people. π₯
* Containers: shows each component in the context view in a more detailed view and how it works, mentioning its technologies without going into more detail. π¦
* Components: going more into detail about each container, describing each component in it. π©
* Code: it is not worth doing because you can automate doing them by your IDE (plantuml), but if you want to diagram this level, you will most probably use UMLs. π»
* Notation: try to be short and meaningful and concise. Be specific and clear about what it is describing. ποΈ
* Acronym: make sure the domain knows about the acronyms you are using. π€
* Elements: visual consistency is essential (using boxes would be useful if it is added with the name, description, and function). Try to keep it short. π
* Lines: try to make it uni-directional and use fewer arrows if possible in multi-directional relation when the result is not vague. Avoid simple descriptions. β‘οΈ
* Making the diagram readable would ensure work is continuous even if the group working on the project changes. π§
* Some tools to work with: plantuml and structurizr. π οΈ

### Chirag Nayyar Video about the free tier πΈ
##### Notes about it:

* Bills Section contains each service and classifies them by region.
* Noticed that the forecast on the homepage is different from the bills section. π€
* You can set alarms from CloudWatch. β°
* 10 alarms are free. π
* I should use tags to categorize resources to make budget analytics better. π·οΈ
### Generating Credentials video

Notes about it:

* CloudShell depends on the region.
* Use`aws --cli-auto-prompt` to make the CLI auto-suggest commands.
* CLI is fun.
* Set up the CLI and updated the Gitpod config.
* Created a budget using the CLI.
* Created an alarm too.

### Security Video

Notes about it:

* Security is gradual and is incremented gradually.
* Added MFA authentication to my root account.
* Enabled CloudTrail.
* Set up Organizations and SCPs.

## Homework Section π

* Link to Conceptual diagram : https://lucid.app/lucidchart/39d55e21-be61-41c3-8378-1d49c0b8181f/edit?viewport_loc=-1070%2C-878%2C2371%2C1312%2C0_0&invitationId=inv_26eae480-c0d3-433b-9689-f1b922e1169d

  ![](assets/week0/cruddur_conceptual_diagram.png)
* Link to Logical Diagram : https://lucid.app/lucidchart/0d14a873-d6bc-47fe-8d4a-0d66b607da3f/edit?view_items=C09x.ijlKOVN&invitationId=inv_1b1419a4-4c03-4856-a447-c979b25fbab5

  ![](assets/week0/Cruddur_Logical_Diagram.png)
* My Napkin Design

  ![](assets/week0/napkin_diagram.jpg)

## Homework Challenges

* destoryed root account and set mfa
  ![](assets/week0/root_user_destruction_and_mfa.png)
* hooked eventbridge to the health dashboard and added it to an sns topic
  ![](assets/week0/event_bridge.png)
* reviewed the questions in the well archeticted framework
* tried to submit a ticket but didn't go through with it

![](assets/week0/ticket.png)

* Architectural Diagram of CI/CD
  Link to it : https://lucid.app/lucidchart/97d006ab-6693-497b-9090-9bfa5db3968c/edit?viewport_loc=99%2C-146%2C2035%2C1312%2C0_0&invitationId=inv_2797e15b-ecfb-4548-a1ca-7a4041b7c8ec

![](assets/week0/blue_green_ci_cd.png)

> Any Proof of work will also be found as a named picture in `assets/week0`
