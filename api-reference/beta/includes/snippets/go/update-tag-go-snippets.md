---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33e35875280d1f11f2070787567fad64b9ba9b7e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084295"
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
graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Patch(options)


```