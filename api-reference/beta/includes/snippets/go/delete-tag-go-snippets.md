---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84e547460c5ac0c3c6710a8d2ecfe57f78a971bc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TagRequestBuilderDeleteQueryParameters{
    Forcedelete: true,
}
options := &msgraphsdk.TagRequestBuilderDeleteOptions{
    Q: requestParameters,
}
caseId := "case-id"
tagId := "tag-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Delete(options)


```