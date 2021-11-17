---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b558757d507215df3b23e94bd2abe0cfded9a6fb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002840"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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