---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba174fa151d963d8320a964965948da28f2c76f4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329155"
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
applicationId := "application-id"
federatedIdentityCredentialId := "federatedIdentityCredential-id"
graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentialsById(&federatedIdentityCredentialId).Patch(requestBody)


```