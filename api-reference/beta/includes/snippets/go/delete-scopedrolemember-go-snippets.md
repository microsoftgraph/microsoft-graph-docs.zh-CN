---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de8b9347bfea45296cc954296bf3d6d166ba2f5f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

administrativeUnitId := "administrativeUnit-id"
scopedRoleMembershipId := "scopedRoleMembership-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembersById(&scopedRoleMembershipId).Delete(options)


```