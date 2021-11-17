---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0282ca8ff2b4a8a0007ccb6010e325925ce18f8a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983442"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageAssignmentResourceRoleId := "accessPackageAssignmentResourceRole-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentResourceRolesById(&accessPackageAssignmentResourceRoleId).Get(options)


```