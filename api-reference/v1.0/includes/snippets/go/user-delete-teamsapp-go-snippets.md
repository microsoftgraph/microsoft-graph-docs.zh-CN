---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50c8bccc14e7e66d5d14773c935e19f77c684b65
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Delete(options)


```