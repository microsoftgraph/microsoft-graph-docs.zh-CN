---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a044b6ed07817b96188a060efabb79d512759a8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328239"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlowAttribute()
displayName := "Hobby"
requestBody.SetDisplayName(&displayName)
description := "Your hobby"
requestBody.SetDescription(&description)
dataType := "string"
requestBody.SetDataType(&dataType)
result, err := graphClient.Identity().UserFlowAttributes().Post(requestBody)


```