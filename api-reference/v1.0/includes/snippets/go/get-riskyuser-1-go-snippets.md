---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a506f7a990bc46df17e12e59e7b4a23569938ee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).Get(nil)


```