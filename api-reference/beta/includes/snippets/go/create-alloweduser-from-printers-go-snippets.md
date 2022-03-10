---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d92d61d3d22418da48ee17b36338f6cdde038b63
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411646"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/{id}",
}
options := &msgraphsdk.UserRequestBuilderPostOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
userId := "user-id"
graphClient.Print().SharesById(&printerShareId).AllowedUsersById(&userId).Post(options)


```