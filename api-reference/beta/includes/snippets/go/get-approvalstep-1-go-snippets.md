---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 697f8ee3c1d7b7fc165e21ff639e0ef4331050c1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982588"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

approvalId := "approval-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).Steps().Get(options)


```