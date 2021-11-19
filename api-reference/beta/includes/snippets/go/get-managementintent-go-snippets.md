---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54b0551128b2c3611863bdfd2e09191f35b8abf1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103307"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementIntentId := "managementIntent-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementIntentsById(&managementIntentId).Get(options)


```