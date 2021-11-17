---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a69d6a55d42248e05e187a8946ee7db377afd055
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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