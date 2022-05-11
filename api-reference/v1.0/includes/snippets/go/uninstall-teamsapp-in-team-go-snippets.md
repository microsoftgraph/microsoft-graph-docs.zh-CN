---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1de6f2fe27b097fb507e328e24bfef52982fb018
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328021"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Delete()


```