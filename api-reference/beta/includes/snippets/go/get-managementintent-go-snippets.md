---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b45ea1f6d63fc64ab678c091b4151c7072e7bc5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managementIntentId := "managementIntent-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementIntentsById(&managementIntentId).Get(options)


```