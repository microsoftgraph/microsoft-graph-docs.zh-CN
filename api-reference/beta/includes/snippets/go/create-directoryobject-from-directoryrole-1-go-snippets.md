---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58175c18da37ebff2c3fba08f016bb83d272e443
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2",
}
directoryRoleId := "directoryRole-id"
directoryObjectId := "directoryObject-id"
graphClient.DirectoryRolesById(&directoryRoleId).MembersById(&directoryObjectId).Post(requestBody)


```