---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebdf58cfac4a1dbfe3d5bbfa72d459408056a7e2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
result, err := graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroups().Get()


```