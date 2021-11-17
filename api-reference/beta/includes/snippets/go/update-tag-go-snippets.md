---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebc6dabee099ba98253a1fea3fd87cdd8917077e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005255"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTag()
description := "This is an updated description."
requestBody.SetDescription(&description)
options := &msgraphsdk.TagRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
tagId := "tag-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Patch(options)


```