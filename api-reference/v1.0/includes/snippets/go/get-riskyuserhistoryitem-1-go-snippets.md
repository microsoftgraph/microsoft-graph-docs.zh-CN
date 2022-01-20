---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4f4a5ff37236eba38589263666f2031e28c7130
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104511"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).History().Get(nil)


```