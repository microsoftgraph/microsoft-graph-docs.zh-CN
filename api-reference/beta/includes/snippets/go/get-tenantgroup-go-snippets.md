---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f85a5fb41fdff4610c8af9193066917bb3156ed
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288986"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantGroupId := "tenantGroup-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroupsById(&tenantGroupId).Get(nil)


```