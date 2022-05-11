---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 856eaad5b39d6fd686753478534d555c252853a7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315475"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrivilegedApproval()
approvalState := "approvalState-value"
requestBody.SetApprovalState(&approvalState)
approverReason := "approverReason-value"
requestBody.SetApproverReason(&approverReason)
privilegedApprovalId := "privilegedApproval-id"
graphClient.PrivilegedApprovalById(&privilegedApprovalId).Patch(requestBody)


```