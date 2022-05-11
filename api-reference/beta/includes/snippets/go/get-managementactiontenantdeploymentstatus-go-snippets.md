---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 579c57af8f9a126902f75c0841e6c1e77df81488
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementActionTenantDeploymentStatusId := "managementActionTenantDeploymentStatus-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatusesById(&managementActionTenantDeploymentStatusId).Get()


```