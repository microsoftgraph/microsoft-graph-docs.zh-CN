---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9b1bf9da9e3d0ea9f85a70c0790e53053156b9f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090017"
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
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignments().Get(options)


```