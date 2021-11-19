---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4196a978b8607c35a3e5ef556e6cc4ea68b39621
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090413"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.UserScopeTeamsAppInstallationRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Get(options)


```