---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f31fe38f7549177d845257fa68a94e0e1fc4d309
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982790"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewApplication()
displayName := "New display name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ApplicationRequestBuilderPatchOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Patch(options)


```