---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edc3d2014491aa977625a9324f9e437d2e763aeb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
directoryRoleId := "directoryRole-id"
result, err := graphClient.DirectoryRolesById(&directoryRoleId).Members().$ref().Post(options)


```