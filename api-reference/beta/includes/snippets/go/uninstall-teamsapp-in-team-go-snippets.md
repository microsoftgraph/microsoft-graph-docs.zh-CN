---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b01335c9ed83341de3b58f9e3ea9b2f56be27d68
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411642"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
result, err := graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Delete(nil)


```