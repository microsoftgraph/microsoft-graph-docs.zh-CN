---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78bdb22c49da784384aa622410ff271aa210356d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089546"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppliesToRequestBuilderGetQueryParameters{
    Select: "id,appId,displayName,createdDateTime",
}
options := &msgraphsdk.AppliesToRequestBuilderGetOptions{
    Q: requestParameters,
}
appManagementPolicyId := "appManagementPolicy-id"
result, err := graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).AppliesTo().Get(options)


```