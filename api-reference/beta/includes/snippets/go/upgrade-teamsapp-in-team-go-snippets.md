---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b40452e9f936438531d085e370f1ba8ece92f826
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Upgrade().Post(options)


```