---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc73596d1e2159d28d99fc24b31a5b167108fb05
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089473"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
name := "Login with the Contoso identity provider"
requestBody.SetName(&name)
type := "OpenIDConnect"
requestBody.SetType(&type)
clientId := "56433757-cadd-4135-8431-2c9e3fd68ae8"
requestBody.SetClientId(&clientId)
clientSecret := "12345"
requestBody.SetClientSecret(&clientSecret)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.openIdConnectProvider",
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid",
}
options := &msgraphsdk.IdentityProvidersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityProviders().Post(options)


```