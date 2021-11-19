---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84767b18ff1e057b8568ed95c13408d1873b0dd1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentResourceRoleId := "accessPackageAssignmentResourceRole-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentResourceRolesById(&accessPackageAssignmentResourceRoleId).Get(options)


```