---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc1aba2fbffa942ca5292e78260d4d7ccad39560
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083192"
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
graphClient.OrganizationById(&organizationId).Branding().Patch(options)


```