---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e54b3fce7f43d7ddd20e5bbd76c8907deb57e42c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBrandingLocalization()
backgroundColor := "#00000F"
requestBody.SetBackgroundColor(&backgroundColor)
signInPageText := "Welcome to Contoso France"
requestBody.SetSignInPageText(&signInPageText)
options := &msgraphsdk.OrganizationalBrandingLocalizationRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
organizationalBrandingLocalizationId := "organizationalBrandingLocalization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).Patch(options)


```