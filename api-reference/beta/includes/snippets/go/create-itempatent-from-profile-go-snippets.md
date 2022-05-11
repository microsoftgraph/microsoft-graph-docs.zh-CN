---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e65f7b1a9845f3ea0561d77e53bd3f3be555809
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329006"
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
result, err := graphClient.Me().Profile().Patents().Post(requestBody)


```