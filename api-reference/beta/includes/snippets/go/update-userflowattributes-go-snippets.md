---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3c6a5b0ee01eb381b0d8ae28209049c7caaec42
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityUserFlowAttribute()
description := "Your new hobby"
requestBody.SetDescription(&description)
options := &msgraphsdk.IdentityUserFlowAttributeRequestBuilderPatchOptions{
    Body: requestBody,
}
identityUserFlowAttributeId := "identityUserFlowAttribute-id"
graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Patch(options)


```