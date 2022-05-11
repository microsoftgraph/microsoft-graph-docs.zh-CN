---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d81f98daf7282913cb086cff982be89da3404753
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326631"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca",
}
directoryRoleId := "directoryRole-id"
directoryObjectId := "directoryObject-id"
graphClient.DirectoryRolesById(&directoryRoleId).MembersById(&directoryObjectId).Post(requestBody)


```