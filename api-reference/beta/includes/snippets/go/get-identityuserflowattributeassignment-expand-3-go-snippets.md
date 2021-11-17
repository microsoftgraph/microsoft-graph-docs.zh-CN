---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83fb4e6391aaa46a9b6385966292506863a0cebc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.IdentityUserFlowAttributeAssignmentRequestBuilderGetOptions{
    Q: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityUserFlowAttributeAssignmentId := "identityUserFlowAttributeAssignment-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignmentsById(&identityUserFlowAttributeAssignmentId).Get(options)


```