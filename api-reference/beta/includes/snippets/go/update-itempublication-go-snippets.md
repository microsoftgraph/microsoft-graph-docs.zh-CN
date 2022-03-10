---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 425e97610a561591ecc0d17f1bb0256471d39254
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412552"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPublication()
publisher := "International Association of Branding Management Publishing"
requestBody.SetPublisher(&publisher)
thumbnailUrl := "https://iabm.io/sdhdfhsdhshsd.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
options := &msgraphsdk.ItemPublicationRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPublicationId := "itemPublication-id"
result, err := graphClient.UsersById(&userId).Profile().PublicationsById(&itemPublicationId).Patch(options)


```