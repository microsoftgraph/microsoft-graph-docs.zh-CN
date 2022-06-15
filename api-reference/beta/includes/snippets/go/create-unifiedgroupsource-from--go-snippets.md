---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6aa26f88d1bf925cf51d067ae4bd7f8c5a1cf98
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedGroupSource()
includedSources := "mailbox"
requestBody.SetIncludedSources(&includedSources)
requestBody.SetAdditionalData(map[string]interface{}{
    "group@odata.bind": "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610",
}
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryCustodianId := "ediscoveryCustodian-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).CustodiansById(&ediscoveryCustodianId).UnifiedGroupSources().Post(requestBody)


```