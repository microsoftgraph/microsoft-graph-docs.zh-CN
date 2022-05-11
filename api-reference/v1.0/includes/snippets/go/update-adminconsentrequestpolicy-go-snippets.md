---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 535c3619e33c37b532e8713497e3d9298cfb0401
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326543"
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
graphClient.Policies().AdminConsentRequestPolicy().Put(requestBody)


```