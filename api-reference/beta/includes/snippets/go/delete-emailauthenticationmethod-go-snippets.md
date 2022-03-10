---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f0a93c2d4d25e38415fb9cb0dfbc34e11e48ba2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412419"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
emailAuthenticationMethodId := "emailAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().EmailMethodsById(&emailAuthenticationMethodId).Delete(nil)


```