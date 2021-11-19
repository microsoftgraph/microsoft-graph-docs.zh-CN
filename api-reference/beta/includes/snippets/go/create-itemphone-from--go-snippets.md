---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67ffc5b714156489ad0a817ccf3e66de27760a8b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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