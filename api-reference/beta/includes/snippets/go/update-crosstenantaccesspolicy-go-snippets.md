---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8fec220c4e6980b78946d1294c499e1d5f50ada
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336611"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicy()
displayName := "CrossTenantAccessPolicy"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.CrossTenantAccessPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().CrossTenantAccessPolicy().Patch(options)


```