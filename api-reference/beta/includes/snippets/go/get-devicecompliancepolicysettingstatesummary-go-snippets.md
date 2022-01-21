---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e6fd19ec79318903ed45399f83167f38ae2a308
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131017"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceCompliancePolicySettingStateSummaryId := "deviceCompliancePolicySettingStateSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().DeviceCompliancePolicySettingStateSummariesById(&deviceCompliancePolicySettingStateSummaryId).Get(nil)


```