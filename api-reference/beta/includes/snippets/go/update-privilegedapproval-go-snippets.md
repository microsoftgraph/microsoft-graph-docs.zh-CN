---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0230ab32fe409bc037071df6c8fe8ef9f65490fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104030"
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
graphClient.PrivilegedApprovalById(&privilegedApprovalId).Patch(options)


```