---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 251bad5c0749d3d4fcde11ede1d7379e0d632395
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202529"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminAccessAssignmentId := "delegatedAdminAccessAssignment-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).AccessAssignmentsById(&delegatedAdminAccessAssignmentId).Get(nil)


```