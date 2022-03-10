---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e15f217999e2592cdd5ce2b887f1bc7fe215bae5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412389"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAssignmentsRequestBody()
requestBody.SetAssignments( []CloudPcProvisioningPolicyAssignment {
    msgraphsdk.NewCloudPcProvisioningPolicyAssignment(),
    SetAdditionalData(map[string]interface{}{
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
options := &msgraphsdk.AssignRequestBuilderPostOptions{
    Body: requestBody,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Assign(cloudPcProvisioningPolicy-id).Post(options)


```