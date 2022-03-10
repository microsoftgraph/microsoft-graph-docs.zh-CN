---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9fd0275704767ef6d063fbfa730d19697c5d43
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412093"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewPolicy()
isGroupOwnerManagementEnabled := true
requestBody.SetIsGroupOwnerManagementEnabled(&isGroupOwnerManagementEnabled)
options := &msgraphsdk.PolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().AccessReviews().Policy().Patch(options)


```