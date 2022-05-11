---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d3d751f994520f48f37bc3c19586c44c4c3a844
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327353"
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
options := &msgraphsdk.BrandingRequestBuilderPatchRequestConfiguration{
    Headers: headers,
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).Branding().PatchWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```