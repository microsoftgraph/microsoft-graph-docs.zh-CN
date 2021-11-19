---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ca62b17f7eba01a73d4984da986c3afbbc7c74d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RiskDetectionsRequestBuilderGetQueryParameters{
    Filter: "riskEventType%20eq%20'unfamiliarFeatures'%20or%20riskLevel%20eq%20'medium'",
}
options := &msgraphsdk.RiskDetectionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskDetections().Get(options)


```