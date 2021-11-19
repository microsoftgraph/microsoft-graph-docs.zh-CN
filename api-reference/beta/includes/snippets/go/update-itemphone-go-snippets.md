---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42a6ecf0bf3fc409e3c51564cce7772ac4aafc41
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093246"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPhone()
type := "other"
requestBody.SetType(&type)
options := &msgraphsdk.ItemPhoneRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPhoneId := "itemPhone-id"
graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Patch(options)


```