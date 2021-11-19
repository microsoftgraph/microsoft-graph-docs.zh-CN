---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5924a9d28f7e3e1a25f6fbabcd981d2bc63c6ce8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
directoryRoleId := "directoryRole-id"
result, err := graphClient.DirectoryRolesById(&directoryRoleId).Members().$ref().Post(options)


```