---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a229a896d191eddf295d3a29c24eed53f000cf7f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099401"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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