---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53935738e1a9f9f7d8fe5189560a24a4296594ef
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012262"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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