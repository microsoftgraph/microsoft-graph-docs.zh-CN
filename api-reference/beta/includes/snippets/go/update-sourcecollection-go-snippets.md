---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9131ee6015cd468c6479128198d4d04659ae375c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSourceCollection()
displayName := "Quarterly Financials search"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.SourceCollectionRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).Patch(options)


```