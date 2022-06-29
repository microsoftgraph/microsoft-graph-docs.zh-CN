---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ad223f561897dc1dfc20a1ebc03d1161398ec82
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694644"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

featureRolloutPolicyId := "featureRolloutPolicy-id"
directoryObjectId := "directoryObject-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).AppliesToById(&directoryObjectId).$ref().Delete()


```