---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a8d61694ff7954dc8ed28aea86606880f3e6968
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412594"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCase()
displayName := "My Case 1 - Renamed"
requestBody.SetDisplayName(&displayName)
description := "Updated description"
requestBody.SetDescription(&description)
externalId := "Updated externalId"
requestBody.SetExternalId(&externalId)
options := &msgraphsdk.CaseRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Patch(options)


```