---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d71c1626fdbd59a5ca51ac1f695ef436d84f882e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019332"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewItemPublication()
description := "One persons journey to the top of the branding management field."
requestBody.SetDescription(&description)
displayName := "Got Brands? The story of Innocenty Popov and his journey to the top."
requestBody.SetDisplayName(&displayName)
publishedDate := "Date"
requestBody.SetPublishedDate(&publishedDate)
publisher := "International Association of Branding Management Publishing"
requestBody.SetPublisher(&publisher)
thumbnailUrl := "https://iabm.io/sdhdfhsdhshsd.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
webUrl := "https://www.iabm.io"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.PublicationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Publications().Post(options)


```