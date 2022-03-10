---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0785933b0abf4581ff0c08f4db34c29223315e5d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412081"
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
applicationId := "application-id"
directoryObjectId := "directoryObject-id"
graphClient.ApplicationsById(&applicationId).OwnersById(&directoryObjectId).Post(options)


```