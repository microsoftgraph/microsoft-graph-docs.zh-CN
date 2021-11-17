---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ed947e03859dd6f90d94a4e8be0411ac346ef52
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020074"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.WorkforceIntegrationRequestBuilderPatchOptions{
    Body: requestBody,
}
workforceIntegrationId := "workforceIntegration-id"
graphClient.Teamwork().WorkforceIntegrationsById(&workforceIntegrationId).Patch(options)


```