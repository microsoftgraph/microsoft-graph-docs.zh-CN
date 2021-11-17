---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f86d23fd5c7b1c838a4c5aa8bf5b4efe8a2d7bc4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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