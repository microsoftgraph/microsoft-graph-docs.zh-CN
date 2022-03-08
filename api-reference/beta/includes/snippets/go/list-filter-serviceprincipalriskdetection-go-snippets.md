---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2bbd75feed26f192ec2a70b01f16ffab9f20a53
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334798"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters{
    Filter: "riskEventType%20eq%20'investigationsThreatIntelligence'%20or%20riskLevel%20eq%20'medium'",
}
options := &msgraphsdk.ServicePrincipalRiskDetectionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityProtection().ServicePrincipalRiskDetections().Get(options)


```