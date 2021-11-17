---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b88f4ac8bedef191c2f9f70378189d5c890ebb17
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990836"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignments().Get(options)


```