---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 066eead4662eb36d5dd9cafe5c3c5b3f7ad678ca
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412257"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalConnection()
name := "Contoso HR Service Tickets"
requestBody.SetName(&name)
description := "Connection to index HR service tickets"
requestBody.SetDescription(&description)
options := &msgraphsdk.ExternalConnectionRequestBuilderPatchOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).Patch(options)


```