---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ea44a2dbfcdc51fc0e6a98feecf7420d5f9fb66
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326803"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminRelationshipOperationId := "delegatedAdminRelationshipOperation-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).OperationsById(&delegatedAdminRelationshipOperationId).Get()


```