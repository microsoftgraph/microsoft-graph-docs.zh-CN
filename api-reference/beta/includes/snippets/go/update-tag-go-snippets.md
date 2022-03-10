---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4f14eaf29cc0da113ca9778fb0fa88526afd899
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412633"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTag()
description := "This is an updated description."
requestBody.SetDescription(&description)
options := &msgraphsdk.TagRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
tagId := "tag-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Patch(options)


```