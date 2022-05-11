---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3b654a56d1a94d2ac496fcd8fbf05b98284bc86
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "enabled": true,
    "timeZone": "America/Chicago",
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Put(requestBody)


```