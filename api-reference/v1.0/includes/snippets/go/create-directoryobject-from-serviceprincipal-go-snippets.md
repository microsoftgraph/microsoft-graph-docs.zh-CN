---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0abb01af626da6bbbd618a426d44e5eacd9c6d29
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
}
servicePrincipalId := "servicePrincipal-id"
directoryObjectId := "directoryObject-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).OwnersById(&directoryObjectId).Post(requestBody)


```