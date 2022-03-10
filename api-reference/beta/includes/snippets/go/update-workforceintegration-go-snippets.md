---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65e618c84a41a8f24991d02a6e2aa526f1be80cd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412011"
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
supports := "supports-value"
requestBody.SetSupports(&supports)
options := &msgraphsdk.WorkforceIntegrationRequestBuilderPatchOptions{
    Body: requestBody,
}
workforceIntegrationId := "workforceIntegration-id"
result, err := graphClient.Teamwork().WorkforceIntegrationsById(&workforceIntegrationId).Patch(options)


```