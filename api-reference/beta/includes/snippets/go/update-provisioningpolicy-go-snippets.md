---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60175796c8309f3936babb3ebc78dbf1714bfef9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412058"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcProvisioningPolicy()
displayName := "HR provisioning policy"
requestBody.SetDisplayName(&displayName)
description := "Provisioning policy for India HR employees"
requestBody.SetDescription(&description)
onPremisesConnectionId := "4e47d0f6-6f77-44f0-8893-c0fe1701b553"
requestBody.SetOnPremisesConnectionId(&onPremisesConnectionId)
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Patch(options)


```