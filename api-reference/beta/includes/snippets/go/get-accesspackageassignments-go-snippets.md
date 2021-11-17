---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0bf805337ad014fba51887fcf21f7b76621de6f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignments().Get(options)


```