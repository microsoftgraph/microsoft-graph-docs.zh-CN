---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7f622b4101f8cd55623501ef68e48b8a2c72484
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411653"
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
result, err := graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Patch(options)


```