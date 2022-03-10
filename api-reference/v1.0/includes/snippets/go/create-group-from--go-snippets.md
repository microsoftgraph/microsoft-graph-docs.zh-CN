---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa08010c2b2b4d8b0044cedb417ba0465276256e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412401"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}",
}
options := &msgraphsdk.GroupRequestBuilderPostOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
groupId := "group-id"
graphClient.Print().SharesById(&printerShareId).AllowedGroupsById(&groupId).Post(options)


```