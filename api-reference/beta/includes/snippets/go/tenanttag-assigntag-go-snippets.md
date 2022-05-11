---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f231e497187ce94e1fd6f81869340c0c042680e3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantIdsRequestBody()
requestBody.SetTenantIds( []String {
    "String",
}
tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).AssignTag(tenantTag-id).Post(requestBody)


```