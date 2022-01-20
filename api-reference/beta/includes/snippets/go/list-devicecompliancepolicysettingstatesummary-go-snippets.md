---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f927199b06720c1eec1e616649eafdde29a46b38
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137129"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.TenantRelationships().ManagedTenants().DeviceCompliancePolicySettingStateSummaries().Get(nil)


```