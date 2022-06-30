---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b48c0555105b02c592fe7149f0a79f3508aefa1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetQueryParameters{
    Select: "id,description,displayName,displayName,domainJoinConfiguration,imageDisplayName,imageId,imageType,onPremisesConnectionId,windowsSettings,managedBy,cloudPcGroupDisplayName,gracePeriodInHours,localAdminEnabled,alternateResourceUrl",
}
options := &msgraphsdk.CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
cloudPcProvisioningPolicyId := "cloudPcProvisioningPolicy-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPoliciesById(&cloudPcProvisioningPolicyId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```