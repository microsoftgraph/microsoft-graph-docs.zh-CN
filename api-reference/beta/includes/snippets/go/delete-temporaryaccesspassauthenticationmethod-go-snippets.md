---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 029feb357dd37adbc545d380d1b003ebde16b701
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
temporaryAccessPassAuthenticationMethodId := "temporaryAccessPassAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethodsById(&temporaryAccessPassAuthenticationMethodId).Delete(nil)


```