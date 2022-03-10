---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f3f7cd1f2a3f54b10738a13651a42dd26b0c020
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412399"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSet()
description := "mySet"
requestBody.SetDescription(&description)
options := &msgraphsdk.SetRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Patch(options)


```