---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e30ea680ee08599e610f6570cd9170c887cc1515
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonWebsite()
requestBody.SetCategories( []String {
    "football",
}
displayName := "Lyn Damer"
requestBody.SetDisplayName(&displayName)
webUrl := "www.lyndamer.no"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.WebsitesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Websites().Post(options)


```