---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0fbd76823aa0ad49ecb95a5d42d8f91489a674c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessReviewPolicy()
isGroupOwnerManagementEnabled := true
requestBody.SetIsGroupOwnerManagementEnabled(&isGroupOwnerManagementEnabled)
options := &msgraphsdk.AccessReviewPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AccessReviewPolicy().Patch(options)


```