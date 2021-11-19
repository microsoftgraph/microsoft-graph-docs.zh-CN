---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eae807658904463f435423b6fe058006ec5e9c3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092367"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlowAttribute()
description := "Your new hobby"
requestBody.SetDescription(&description)
options := &msgraphsdk.IdentityUserFlowAttributeRequestBuilderPatchOptions{
    Body: requestBody,
}
identityUserFlowAttributeId := "identityUserFlowAttribute-id"
graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Patch(options)


```