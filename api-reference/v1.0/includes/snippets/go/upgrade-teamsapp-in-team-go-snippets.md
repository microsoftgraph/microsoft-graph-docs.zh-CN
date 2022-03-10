---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a72126e1ccab8a89d8e18dee67b9bee17f076f9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412508"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Upgrade(team-id, teamsAppInstallation-id).Post(nil)


```