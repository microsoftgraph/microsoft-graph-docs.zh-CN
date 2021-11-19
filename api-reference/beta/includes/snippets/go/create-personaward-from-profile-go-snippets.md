---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 172207bb04c36d3ecd68e33a4886f373b8834f30
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103205"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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