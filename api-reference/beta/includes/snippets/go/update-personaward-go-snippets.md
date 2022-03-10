---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81c6713cc9f2fe99d31fc166f3f952c8f0090b08
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412666"
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
result, err := graphClient.UsersById(&userId).Profile().AwardsById(&personAwardId).Patch(options)


```