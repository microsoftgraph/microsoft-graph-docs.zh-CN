---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9271bf14f628d2120c406441286626ff8858ce12
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
description := "World's greatest football club"
requestBody.SetDescription(&description)
displayName := "Chelsea FC"
requestBody.SetDisplayName(&displayName)
webUrl := "https://www.chelseafc.com"
requestBody.SetWebUrl(&webUrl)
result, err := graphClient.Me().Profile().Interests().Post(requestBody)


```