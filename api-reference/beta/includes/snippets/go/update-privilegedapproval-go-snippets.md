---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4168f242f7c89d7ccd55d151e53eb2959a45d80c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63671431"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrivilegedApproval()
approvalState := "approvalState-value"
requestBody.SetApprovalState(&approvalState)
approverReason := "approverReason-value"
requestBody.SetApproverReason(&approverReason)
options := &msgraphsdk.PrivilegedApprovalRequestBuilderPatchOptions{
    Body: requestBody,
}
privilegedApprovalId := "privilegedApproval-id"
result, err := graphClient.PrivilegedApprovalById(&privilegedApprovalId).Patch(options)


```