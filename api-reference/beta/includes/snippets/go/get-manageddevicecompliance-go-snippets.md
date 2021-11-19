---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 379dcc9310204c8f33aae901a3003033d7ac6c33
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097071"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceComplianceId := "managedDeviceCompliance-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceCompliancesById(&managedDeviceComplianceId).Get(options)


```