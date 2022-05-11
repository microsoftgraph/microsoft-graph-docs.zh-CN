---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6949b8935c53ec5404f4a9b6610bd766cbdd04e5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceCompliancePolicySettingStateSummaryId := "deviceCompliancePolicySettingStateSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().DeviceCompliancePolicySettingStateSummariesById(&deviceCompliancePolicySettingStateSummaryId).Get()


```