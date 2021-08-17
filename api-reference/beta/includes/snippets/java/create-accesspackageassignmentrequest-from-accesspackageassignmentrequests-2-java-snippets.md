---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcf805e8d12855155f36c38a083620d3ae6f775a
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368865"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = new AccessPackageAssignmentRequest();
accessPackageAssignmentRequest.requestType = "UserAdd";
AccessPackageAssignment accessPackageAssignment = new AccessPackageAssignment();
accessPackageAssignment.targetId = "46184453-e63b-4f20-86c2-c557ed5d5df9";
accessPackageAssignment.assignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8";
accessPackageAssignment.accessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b";
accessPackageAssignmentRequest.accessPackageAssignment = accessPackageAssignment;
LinkedList<AccessPackageAnswer> answersList = new LinkedList<AccessPackageAnswer>();
AccessPackageAnswerString answers = new AccessPackageAnswerString();
answers.value = "Arizona";
AccessPackageMultipleChoiceQuestion answeredQuestion = new AccessPackageMultipleChoiceQuestion();
answeredQuestion.id = "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF";
answers.answeredQuestion = answeredQuestion;
answersList.add(answers);
AccessPackageAnswerString answers1 = new AccessPackageAnswerString();
answers1.value = "Need access to marketing campaign material";
AccessPackageTextInputQuestion answeredQuestion1 = new AccessPackageTextInputQuestion();
answeredQuestion1.id = "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA";
answers1.answeredQuestion = answeredQuestion1;
answersList.add(answers1);
accessPackageAssignmentRequest.answers = answersList;

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .post(accessPackageAssignmentRequest);

```