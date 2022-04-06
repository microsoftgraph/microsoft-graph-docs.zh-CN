---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac9ea8effcea402b9acd0355c1a4b6afac99a792
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528155"
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
graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).Patch(options)


```