---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6bb8556baf274931f4e3fe1bf16b85b2e2bb58b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminRelationshipRequestId := "delegatedAdminRelationshipRequest-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).RequestsById(&delegatedAdminRelationshipRequestId).Get(nil)


```