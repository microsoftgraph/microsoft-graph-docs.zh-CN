---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc1a96891d9e9d9b3c3349348a19357ebdd7075d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096338"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemEmail()
displayName := "Business Email"
requestBody.SetDisplayName(&displayName)
type := "work"
requestBody.SetType(&type)
options := &msgraphsdk.ItemEmailRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemEmailId := "itemEmail-id"
graphClient.UsersById(&userId).Profile().EmailsById(&itemEmailId).Patch(options)


```