---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 196ec56e0f06c10c22049995e6e93c84a0528be4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managedDeviceComplianceTrendId := "managedDeviceComplianceTrend-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceComplianceTrendsById(&managedDeviceComplianceTrendId).Get(options)


```