---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92054679eab463bdd7af9f03443acefd92b3cc36
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104058"
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
options := &msgraphsdk.TagsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Tags().Post(options)


```