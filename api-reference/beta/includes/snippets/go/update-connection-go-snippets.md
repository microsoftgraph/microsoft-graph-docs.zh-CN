---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313aba4020991d9a50f173b81bafffe8bc843854
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034446"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewExternalConnection()
name := "Contoso HR Service Tickets"
requestBody.SetName(&name)
description := "Connection to index HR service tickets"
requestBody.SetDescription(&description)
options := &msgraphsdk.ExternalConnectionRequestBuilderPatchOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Patch(options)


```