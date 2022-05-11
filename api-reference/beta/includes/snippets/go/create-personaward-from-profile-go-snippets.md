---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5f0441e76e96faa6f3b10d18643ba596ac6f6d8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325843"
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
result, err := graphClient.Me().Profile().Awards().Post(requestBody)


```