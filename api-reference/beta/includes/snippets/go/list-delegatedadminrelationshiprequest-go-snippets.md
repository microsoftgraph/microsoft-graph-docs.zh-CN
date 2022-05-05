---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d45d2be21da88058759c99f974347a32dc86336
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203515"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).Requests().Get(nil)


```