---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad564678f8c4016c1ec6650d30ce2c03795ba9db
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329146"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantIdRequestBody()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroups().TenantSearch().Post(requestBody)


```