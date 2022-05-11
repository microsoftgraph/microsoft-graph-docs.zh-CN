---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58fac57e3024b6a165b8df22200759c777c24386
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329084"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).History().Get()


```