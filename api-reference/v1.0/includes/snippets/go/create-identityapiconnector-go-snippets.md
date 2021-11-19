---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 388e9e3fb7fcd3269cf8b9ecc8772d4c82f28b86
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityApiConnector()
displayName := "Test API"
requestBody.SetDisplayName(&displayName)
targetUrl := "https://someotherapi.com/api"
requestBody.SetTargetUrl(&targetUrl)
authenticationConfiguration := msgraphsdk.NewApiAuthenticationConfigurationBase()
requestBody.SetAuthenticationConfiguration(authenticationConfiguration)
authenticationConfiguration.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "CertificatePassword",
}
options := &msgraphsdk.ApiConnectorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ApiConnectors().Post(options)


```