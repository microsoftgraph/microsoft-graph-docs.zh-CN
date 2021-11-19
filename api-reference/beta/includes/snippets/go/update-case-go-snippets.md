---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6406d8e1776e847b9b4da081ed19e0ffe5e93079
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095861"
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
graphClient.Compliance().Ediscovery().CasesById(&caseId).Patch(options)


```