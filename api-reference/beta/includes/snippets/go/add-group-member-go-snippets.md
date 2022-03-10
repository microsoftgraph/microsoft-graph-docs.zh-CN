---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 207d072195d668b6a869bcc197fccf1f012c46c5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412253"
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
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).MembersById(&directoryObjectId).Post(options)


```