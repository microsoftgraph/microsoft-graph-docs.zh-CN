---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e181fd4940527bffe45667e1e2f8bda2ae3b2023
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLanguageProficiency()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.LanguageProficiencyRequestBuilderPatchOptions{
    Body: requestBody,
}
languageProficiencyId := "languageProficiency-id"
graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Patch(options)


```