---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb4c4da92d82f4f3fcaf2693fc1dc890d0318552
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081640"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserScopeTeamsAppInstallation()
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
}
options := &msgraphsdk.InstalledAppsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledApps().Post(options)


```