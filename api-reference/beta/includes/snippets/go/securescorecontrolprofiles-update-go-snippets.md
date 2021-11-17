---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a096fd3c8ec3a943cae47d3946d5e82bddcad7cc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSecureScoreControlProfile()
controlStateUpdates := "controlStateUpdates-value"
requestBody.SetControlStateUpdates(&controlStateUpdates)
options := &msgraphsdk.SecureScoreControlProfileRequestBuilderPatchOptions{
    Body: requestBody,
}
secureScoreControlProfileId := "secureScoreControlProfile-id"
graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(options)


```