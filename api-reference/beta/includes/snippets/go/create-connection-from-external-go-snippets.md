---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1677447d7bb735472906a7f0f2303b5e9078a843
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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