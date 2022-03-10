---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e918fe100aca00f0d9c3a5dd8a70ed0067158db
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412050"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderPostOptions{
    Body: requestBody,
}
deviceId := "device-id"
directoryObjectId := "directoryObject-id"
graphClient.DevicesById(&deviceId).RegisteredOwnersById(&directoryObjectId).Post(options)


```