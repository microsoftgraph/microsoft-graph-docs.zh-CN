---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10e6de565723922734fbc985b867ccb81e5f778f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084407"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWorkforceIntegration()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
apiVersion := int32(99)
requestBody.SetApiVersion(&apiVersion)
encryption := msgraphsdk.NewWorkforceIntegrationEncryption()
requestBody.SetEncryption(encryption)
protocol := "protocol-value"
encryption.SetProtocol(&protocol)
secret := "secret-value"
encryption.SetSecret(&secret)
isActive := true
requestBody.SetIsActive(&isActive)
url := "url-value"
requestBody.SetUrl(&url)
supportedEntities := "supportedEntities-value"
requestBody.SetSupportedEntities(&supportedEntities)
options := &msgraphsdk.WorkforceIntegrationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Teamwork().WorkforceIntegrations().Post(options)


```