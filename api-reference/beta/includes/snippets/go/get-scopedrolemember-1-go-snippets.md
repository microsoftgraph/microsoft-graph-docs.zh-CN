---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19858f9cdc53a77c453820068f8bf40139de3116
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987522"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

administrativeUnitId := "administrativeUnit-id"
scopedRoleMembershipId := "scopedRoleMembership-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembersById(&scopedRoleMembershipId).Get(options)


```