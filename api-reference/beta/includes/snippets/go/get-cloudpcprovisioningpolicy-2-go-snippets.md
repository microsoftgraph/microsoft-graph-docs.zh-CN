---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 226ed17d015f46a4631a1a7ec96750561ba9418b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetQueryParameters{
    Expand: "assignments",
}
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```