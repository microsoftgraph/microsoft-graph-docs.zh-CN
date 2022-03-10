---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e204fbb734b7e892d27babd534e3b5e4f1e5503
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDisplayNameRequestBody()
displayName := "My custom name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.InstantiateRequestBuilderPostOptions{
    Body: requestBody,
}
applicationTemplateId := "applicationTemplate-id"
result, err := graphClient.ApplicationTemplatesById(&applicationTemplateId).Instantiate(applicationTemplate-id).Post(options)


```