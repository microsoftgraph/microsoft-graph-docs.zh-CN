---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f325ed8bbb84d62ab1db09a2ebd85246f8665f8b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988258"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequestsById(&accessPackageAssignmentRequestId).Delete(options)


```