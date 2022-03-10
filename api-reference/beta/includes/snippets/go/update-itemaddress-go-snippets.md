---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9018db0d6f6e89293a43075079f71a6df6cf7128
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemAddress()
allowedAudiences := "me"
requestBody.SetAllowedAudiences(&allowedAudiences)
displayName := "Secret Hideout"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ItemAddressRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemAddressId := "itemAddress-id"
result, err := graphClient.UsersById(&userId).Profile().AddressesById(&itemAddressId).Patch(options)


```