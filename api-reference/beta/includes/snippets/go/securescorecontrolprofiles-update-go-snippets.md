---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38c22c11d134b82286ed228743e8476319a67a3c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412491"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecureScoreControlProfile()
controlStateUpdates := "controlStateUpdates-value"
requestBody.SetControlStateUpdates(&controlStateUpdates)
options := &msgraphsdk.SecureScoreControlProfileRequestBuilderPatchOptions{
    Body: requestBody,
}
secureScoreControlProfileId := "secureScoreControlProfile-id"
result, err := graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(options)


```