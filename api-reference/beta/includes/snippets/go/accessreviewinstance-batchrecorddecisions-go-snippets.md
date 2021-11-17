---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3853384bf49ca115490c37a9dfa05c2d5f96cc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
decision := "Approve"
requestBody.SetDecision(&decision)
justification := "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team"
requestBody.SetJustification(&justification)
resourceId := "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
requestBody.SetResourceId(&resourceId)
options := &msgraphsdk.BatchRecordDecisionsRequestBuilderPostOptions{
    Body: requestBody,
}
accessReviewInstanceId := "accessReviewInstance-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).BatchRecordDecisions().Post(options)


```