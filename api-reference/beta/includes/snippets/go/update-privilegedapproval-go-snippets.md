---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8af4ba51b27b3fe94a76ddd1654331359bfcc110
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980374"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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