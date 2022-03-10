---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8bd3469004d4fa19ca1686589046a5bfb9cac8d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/groups/{id}",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
directoryObjectId := "directoryObject-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).MembersById(&directoryObjectId).Post(options)


```