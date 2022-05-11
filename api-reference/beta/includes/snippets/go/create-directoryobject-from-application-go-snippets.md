---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea216016d35d6330e4cb25192a5e635d7143a080
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326302"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}",
}
applicationId := "application-id"
directoryObjectId := "directoryObject-id"
graphClient.ApplicationsById(&applicationId).OwnersById(&directoryObjectId).Post(requestBody)


```