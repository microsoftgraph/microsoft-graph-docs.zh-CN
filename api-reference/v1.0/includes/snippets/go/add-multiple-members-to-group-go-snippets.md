---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: facc5236ae523ea40af4bf5c729579f399cebcc5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
requestBody.SetAdditionalData(map[string]interface{}{
    "members@odata.bind":  []String {
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
        "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    }
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(requestBody)


```