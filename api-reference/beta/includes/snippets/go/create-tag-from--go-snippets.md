---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 295bb6cf34923deb0c832c6bd07c1819d79b4b92
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020942"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTag()
displayName := "Privileged"
requestBody.SetDisplayName(&displayName)
description := "The document is privileged"
requestBody.SetDescription(&description)
requestBody.SetAdditionalData(map[string]interface{}{
    "parent@odata.bind": "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3",
}
options := &msgraphsdk.TagsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Tags().Post(options)


```