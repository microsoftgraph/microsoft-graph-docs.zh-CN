---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69309d69e86f96393a633d56f069fc68bae1e153
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348385"
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
graphClient.Teamwork().DevicesById(&teamworkDeviceId).UpdateSoftware().Post(options)


```