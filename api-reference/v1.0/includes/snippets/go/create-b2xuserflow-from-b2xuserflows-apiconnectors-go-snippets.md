---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a705d2cb4273d971a9da37d2dcca096cbbe4b8f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087055"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2xIdentityUserFlow()
id := "UserFlowWithAPIConnector"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(1)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
apiConnectorConfiguration := msgraphsdk.NewUserFlowApiConnectorConfiguration()
requestBody.SetApiConnectorConfiguration(apiConnectorConfiguration)
postFederationSignup := msgraphsdk.NewIdentityApiConnector()
apiConnectorConfiguration.SetPostFederationSignup(postFederationSignup)
postFederationSignup.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}",
}
postAttributeCollection := msgraphsdk.NewIdentityApiConnector()
apiConnectorConfiguration.SetPostAttributeCollection(postAttributeCollection)
postAttributeCollection.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}",
}
options := &msgraphsdk.B2xUserFlowsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().B2xUserFlows().Post(options)


```