---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f116713c621248598f086460b57e807fa6b26ea
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonCertification()
certificationId := "KB-1235466333663322"
requestBody.SetCertificationId(&certificationId)
description := "Blackbelt in Marketing - Brand Management"
requestBody.SetDescription(&description)
displayName := "Marketing Blackbelt - Brand Management"
requestBody.SetDisplayName(&displayName)
thumbnailUrl := "https://iame.io/dfhdfdfd334.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
webUrl := "https://www.iame.io/blackbelt"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.CertificationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Certifications().Post(options)


```