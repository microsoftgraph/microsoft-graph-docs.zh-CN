---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6761bd0b8f694cc36ee354c48b28ef4c36ef2a8b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988391"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSet()
description := "mySet"
requestBody.SetDescription(&description)
options := &msgraphsdk.SetRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
setId := "set-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Patch(options)


```