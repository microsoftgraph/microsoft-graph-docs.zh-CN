---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a40fe62de18fb972e3b6533a03e3d0b172c58934
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411829"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

approvalId := "approval-id"
approvalStepId := "approvalStep-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).StepsById(&approvalStepId).Patch(nil)


```