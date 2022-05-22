---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f833fef4a3f4ce96bb6fe6ff3f2a872bdb91b431
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629799"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).Delete()


```