---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3e81342538d57fd85794faf5743422bdbcbeb9e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087407"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "isEnabled": true,
    "notifyReviewers": true,
    "remindersEnabled": true,
    "requestDurationInDays": ,
    "reviewers":  []Object {
    }
}
options := &msgraphsdk.AdminConsentRequestPolicyRequestBuilderPutOptions{
    Body: requestBody,
}
graphClient.Policies().AdminConsentRequestPolicy().Put(options)


```