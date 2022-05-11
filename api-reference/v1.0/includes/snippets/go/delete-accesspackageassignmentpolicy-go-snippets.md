---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03b7266324158c6456d85cd5fe5aa59c85243561
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328986"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
graphClient.IdentityGovernance().EntitlementManagement().AssignmentPoliciesById(&accessPackageAssignmentPolicyId).Delete()


```