---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ea4efd6bbc89a0d0d6246921c85e0d6d4b19b23
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66604498"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicy()
requestBody.SetAllowedCloudEndpoints( []String {
    "microsoftonline.us",
    "partner.microsoftonline.cn",
}
graphClient.Policies().CrossTenantAccessPolicy().Patch(requestBody)


```