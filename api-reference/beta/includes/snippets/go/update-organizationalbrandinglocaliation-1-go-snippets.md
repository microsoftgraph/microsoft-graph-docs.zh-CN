---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea21baa5d11ea0b276806a34f4109f567dcf5649
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412754"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBranding()
signInPageText := "Default"
requestBody.SetSignInPageText(&signInPageText)
usernameHintText := "DefaultHint"
requestBody.SetUsernameHintText(&usernameHintText)
headers := map[string]string{
    "Accept-Language": "0"
}
options := &msgraphsdk.BrandingRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Patch(options)


```