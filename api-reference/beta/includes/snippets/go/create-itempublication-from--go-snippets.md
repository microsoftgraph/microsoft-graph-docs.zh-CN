---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59ff3f2a711d3d51fd5780d6c2f720d969f08c94
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102927"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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