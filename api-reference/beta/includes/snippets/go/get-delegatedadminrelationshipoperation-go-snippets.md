---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c6d0b61a0223226e4622a61879ae465a8c88919
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204103"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminRelationshipOperationId := "delegatedAdminRelationshipOperation-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).OperationsById(&delegatedAdminRelationshipOperationId).Get(nil)


```