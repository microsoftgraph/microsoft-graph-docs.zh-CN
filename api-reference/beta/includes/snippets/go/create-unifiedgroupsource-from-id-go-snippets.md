---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8c5a43550e6a68a6662f52c6e0f9eb2e76af68a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedGroupSource()
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
requestBody.SetAdditionalData(map[string]interface{}{
    "group@odata.bind": "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84",
}
options := &msgraphsdk.UnifiedGroupSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSources().Post(options)


```