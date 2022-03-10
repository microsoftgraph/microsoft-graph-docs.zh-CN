---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf49bc42f37daf43d82fbb49ee2501192b3ae00f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412286"
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
setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Patch(options)


```