---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81c5f0009a83d137266976b923bc32af334c8bfa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101585"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().Get(options)


```