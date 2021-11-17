---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e50c87b66e8ef2873d9c9c38ba11e6210e636eb6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983532"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPolicies().Get(options)


```