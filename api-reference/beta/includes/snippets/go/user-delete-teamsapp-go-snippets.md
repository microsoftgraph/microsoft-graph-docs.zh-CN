---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36b825d7085124d91a54c42e8a592186eec8e628
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Delete(options)


```