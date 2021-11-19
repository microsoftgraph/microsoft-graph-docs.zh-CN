---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd506591eda73b66c334cb5c2923913db8fbc2cd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092127"
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
graphClient.External().ConnectionsById(&externalConnectionId).Patch(options)


```