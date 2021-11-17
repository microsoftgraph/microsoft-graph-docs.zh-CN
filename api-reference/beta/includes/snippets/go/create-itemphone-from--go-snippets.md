---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7f8ab68c0aca587c6a7ae48de8ecd25bb6d780f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewItemPhone()
displayName := "Car Phone"
requestBody.SetDisplayName(&displayName)
number := "+7 499 342 22 13"
requestBody.SetNumber(&number)
options := &msgraphsdk.PhonesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Phones().Post(options)


```