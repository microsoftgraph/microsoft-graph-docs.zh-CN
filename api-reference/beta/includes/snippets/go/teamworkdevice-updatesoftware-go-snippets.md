---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a764cef7f54e3ba75c564cc3cc4d0e146f4edb2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
softwareType := "teamsClient"
requestBody.SetSoftwareType(&softwareType)
softwareVersion := "1.0.96.22"
requestBody.SetSoftwareVersion(&softwareVersion)
options := &msgraphsdk.UpdateSoftwareRequestBuilderPostOptions{
    Body: requestBody,
}
teamworkDeviceId := "teamworkDevice-id"
graphClient.Teamwork().DevicesById(&teamworkDeviceId).UpdateSoftware(teamworkDevice-id).Post(options)


```