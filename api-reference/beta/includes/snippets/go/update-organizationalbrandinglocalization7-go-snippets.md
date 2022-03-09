---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81bc1cba76e1d52d77178765fd08776fe4a79c99
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBrandingLocalization()
signInPageText := "Welcome to Contoso France."
requestBody.SetSignInPageText(&signInPageText)
usernameHintText := " "
requestBody.SetUsernameHintText(&usernameHintText)
options := &msgraphsdk.OrganizationalBrandingLocalizationRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
organizationalBrandingLocalizationId := "organizationalBrandingLocalization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).Patch(options)


```