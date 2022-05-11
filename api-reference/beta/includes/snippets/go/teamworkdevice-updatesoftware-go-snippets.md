---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c01be37f21b72a180ec56ce4b7bee3882d06c3c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328992"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
softwareType := "teamsClient"
requestBody.SetSoftwareType(&softwareType)
softwareVersion := "1.0.96.22"
requestBody.SetSoftwareVersion(&softwareVersion)
teamworkDeviceId := "teamworkDevice-id"
graphClient.Teamwork().DevicesById(&teamworkDeviceId).UpdateSoftware(teamworkDevice-id).Post(requestBody)


```