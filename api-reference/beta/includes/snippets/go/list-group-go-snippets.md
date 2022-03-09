---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87953fc94157889510d4e4f02b3b968f2e2eb2b5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394780"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
result, err := graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroups().Get(nil)


```