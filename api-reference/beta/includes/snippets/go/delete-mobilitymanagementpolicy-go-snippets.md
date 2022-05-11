---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90658121503c77af190914546fab7ec0532ecada
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).Delete()


```