---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd35d851e4459a03375e14b3e1c61ee990d27d20
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329180"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentitySecurityDefaultsEnforcementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
graphClient.Policies().IdentitySecurityDefaultsEnforcementPolicy().Patch(requestBody)


```