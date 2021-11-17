---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aca84e1bded093ea30c748f843c713af44ee5636
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975650"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetQueryParameters{
    Expand: "assignments",
}
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetOptions{
    Q: requestParameters,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).Get(options)


```