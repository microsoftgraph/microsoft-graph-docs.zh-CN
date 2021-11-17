---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562fd671da61427eb67ea1ee3fc62f08f1847481
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974886"
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
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().SetOrder().Post(options)


```