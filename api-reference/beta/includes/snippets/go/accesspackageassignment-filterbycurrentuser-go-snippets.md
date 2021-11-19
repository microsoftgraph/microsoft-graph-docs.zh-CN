---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7319e65850db06283cd4a9c8ccc10d8ba7feedff
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084221"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentsById(&accessPackageAssignmentId).Get(options)


```