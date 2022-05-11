---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82afb01ea3fa6fe650a79a800e9b322776364fe5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328809"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTag()
displayName := "Privileged"
requestBody.SetDisplayName(&displayName)
description := "The document is privileged"
requestBody.SetDescription(&description)
requestBody.SetAdditionalData(map[string]interface{}{
    "parent@odata.bind": "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3",
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Tags().Post(requestBody)


```