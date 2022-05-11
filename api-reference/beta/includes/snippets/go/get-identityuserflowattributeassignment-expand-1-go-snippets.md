---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07fae4b0a2d68987d293dc2882e97ba37f86df7f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```