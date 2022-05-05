---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971e01f38cee077f89f25f19ece3520a49e12b26
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209897"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentPoliciesById(&accessPackageAssignmentPolicyId).Get(nil)


```