---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9bcb62811241bd526154e967ec7ef61ac0cfd30
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
result, err := graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).Get(options)


```