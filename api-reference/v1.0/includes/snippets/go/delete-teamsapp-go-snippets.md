---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 156bced3cee2ccc1db70619073ecbe666ac54c05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).Delete()


```