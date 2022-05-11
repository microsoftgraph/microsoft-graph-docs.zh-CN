---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a77d5fe6150e2910ed22aa749bfe930eacad4aff
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326880"
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
result, err := graphClient.Me().Profile().Publications().Post(requestBody)


```