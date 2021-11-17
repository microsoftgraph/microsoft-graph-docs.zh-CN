---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3548b423f2d6d5388d5917be248fe2423192de5e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023651"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewItemPatent()
description := "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel."
requestBody.SetDescription(&description)
displayName := "Inferring User Intent through browsing behaviors"
requestBody.SetDisplayName(&displayName)
isPending := true
requestBody.SetIsPending(&isPending)
number := "USPTO-3954432633"
requestBody.SetNumber(&number)
webUrl := "https://patents.gov/3954432633"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.PatentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Patents().Post(options)


```