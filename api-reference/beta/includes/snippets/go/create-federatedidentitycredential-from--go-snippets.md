---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24095fe5724a6b35621d806484e7cd0c0d5d6783
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092584"
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
requestBody.SetAudiences( []String {
    "api://AzureADTokenExchange",
}
options := &msgraphsdk.FederatedIdentityCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).FederatedIdentityCredentials().Post(options)


```