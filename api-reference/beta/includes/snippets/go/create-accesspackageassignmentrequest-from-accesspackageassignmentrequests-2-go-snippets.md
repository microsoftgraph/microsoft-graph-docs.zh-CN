---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17c1c1577e1e9720cd13026a34e3fdc91d399ca8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098685"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "UserAdd"
requestBody.SetRequestType(&requestType)
accessPackageAssignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAccessPackageAssignment(accessPackageAssignment)
targetId := "46184453-e63b-4f20-86c2-c557ed5d5df9"
accessPackageAssignment.SetTargetId(&targetId)
assignmentPolicyId := "2264bf65-76ba-417b-a27d-54d291f0cbc8"
accessPackageAssignment.SetAssignmentPolicyId(&assignmentPolicyId)
accessPackageId := "a914b616-e04e-476b-aa37-91038f0b165b"
accessPackageAssignment.SetAccessPackageId(&accessPackageId)
requestBody.SetAnswers( []AccessPackageAnswer {
    msgraphsdk.NewAccessPackageAnswer(),
answeredQuestion := msgraphsdk.NewAccessPackageQuestion()
    SetAnsweredQuestion(answeredQuestion)
id := "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
    answeredQuestion.SetId(&id)
    answeredQuestion.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
    }
    msgraphsdk.NewAccessPackageAnswer(),
answeredQuestion := msgraphsdk.NewAccessPackageQuestion()
    SetAnsweredQuestion(answeredQuestion)
id := "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
    answeredQuestion.SetId(&id)
    answeredQuestion.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
    }
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().Post(requestBody)


```