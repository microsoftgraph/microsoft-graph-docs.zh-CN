---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 949226c03d3ef671aac436b1ee2ed7ae390a99b9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104256"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAward()
issuingAuthority := "International Association of Branding Management"
requestBody.SetIssuingAuthority(&issuingAuthority)
thumbnailUrl := "https://iabm.io/sdhdfhsdhshsd.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
options := &msgraphsdk.PersonAwardRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
personAwardId := "personAward-id"
graphClient.UsersById(&userId).Profile().AwardsById(&personAwardId).Patch(options)


```