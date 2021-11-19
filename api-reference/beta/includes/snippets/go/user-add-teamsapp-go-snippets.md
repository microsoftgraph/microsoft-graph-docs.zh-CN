---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 602ac10d3656a76da9336532099a673f4f4b226b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091902"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserScopeTeamsAppInstallation()
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
}
options := &msgraphsdk.InstalledAppsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledApps().Post(options)


```