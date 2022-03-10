---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bc0a1df7f0ecefb8b8924743ac8c310017f8877
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFederatedIdentityCredential()
name := "testing02"
requestBody.SetName(&name)
issuer := "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0"
requestBody.SetIssuer(&issuer)
subject := "a7d388c3-5e3f-4959-ac7d-786b3383006a"
requestBody.SetSubject(&subject)
description := "Updated description"
requestBody.SetDescription(&description)
requestBody.SetAudiences( []String {
    "api://AzureADTokenExchange",
}
options := &msgraphsdk.FederatedIdentityCredentialRequestBuilderPatchOptions{
    Body: requestBody,
}
applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Patch(options)


```