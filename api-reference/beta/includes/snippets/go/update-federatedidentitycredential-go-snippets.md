---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 260382f829b9b11d33347cbad8f6fa46dfe54289
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034418"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Patch(options)


```