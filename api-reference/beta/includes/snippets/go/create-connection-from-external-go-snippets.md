---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 732f279a3886cd7168794d1e367355e8136532c5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101174"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalConnection()
id := "contosohr"
requestBody.SetId(&id)
name := "Contoso HR"
requestBody.SetName(&name)
description := "Connection to index Contoso HR system"
requestBody.SetDescription(&description)
options := &msgraphsdk.ConnectionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.External().Connections().Post(options)


```