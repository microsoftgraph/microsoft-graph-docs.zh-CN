---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a43eaf763a1d006e9ffc921a7c1d7c4f4a62e318
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096374"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
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
graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Assign().Post(options)


```