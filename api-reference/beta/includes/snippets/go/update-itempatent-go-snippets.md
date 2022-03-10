---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeeff4b9aca3fe0e55b16632ea45429f7f848618
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411654"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPatent()
number := "USPTO-3954432633"
requestBody.SetNumber(&number)
webUrl := "https://patents.gov/3954432633"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.ItemPatentRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPatentId := "itemPatent-id"
result, err := graphClient.UsersById(&userId).Profile().PatentsById(&itemPatentId).Patch(options)


```