---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1ac7e0fdcd81a455e51326670864db06ccb5f2f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
    "password": "<password>",
}
options := &msgraphsdk.ApiConnectorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ApiConnectors().Post(options)


```