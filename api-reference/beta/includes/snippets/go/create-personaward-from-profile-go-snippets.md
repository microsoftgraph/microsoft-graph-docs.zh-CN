---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7892625c4e83538c64f87a0e6d6ad17b852674a6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027949"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonAward()
description := "Lifetime Achievement award from the International Association of Branding Managers"
requestBody.SetDescription(&description)
displayName := "Lifetime Achievement Award For Excellence in Branding"
requestBody.SetDisplayName(&displayName)
issuedDate := "Date"
requestBody.SetIssuedDate(&issuedDate)
issuingAuthority := "International Association of Branding Management"
requestBody.SetIssuingAuthority(&issuingAuthority)
thumbnailUrl := "https://iabm.io/sdhdfhsdhshsd.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
webUrl := "https://www.iabm.io"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.AwardsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Awards().Post(options)


```