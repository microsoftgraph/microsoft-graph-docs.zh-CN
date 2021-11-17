---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4375cfc0bddf63b3f296ad69ef342ae378b48da7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021348"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
newAssignmentOrder := msgraphsdk.NewAssignmentOrder()
requestBody.SetNewAssignmentOrder(newAssignmentOrder)
newAssignmentOrder.SetOrder( []String {
    "City",
    "extension_GUID_ShoeSize",
}
options := &msgraphsdk.SetOrderRequestBuilderPostOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignments().SetOrder().Post(options)


```