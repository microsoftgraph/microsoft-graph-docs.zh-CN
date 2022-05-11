---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba64aa37c0af835e1d318f2aecffcdb2b34a0d24
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewApprovalStage()
reviewResult := "Approve"
requestBody.SetReviewResult(&reviewResult)
justification := "OK"
requestBody.SetJustification(&justification)
approvalId := "approval-id"
approvalStageId := "approvalStage-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).StagesById(&approvalStageId).Patch(requestBody)


```