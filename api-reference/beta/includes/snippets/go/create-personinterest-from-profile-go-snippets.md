---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 712b54289c1700e69d0e0cfdb8dead24d9a91220
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090305"
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
options := &msgraphsdk.InterestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Interests().Post(options)


```