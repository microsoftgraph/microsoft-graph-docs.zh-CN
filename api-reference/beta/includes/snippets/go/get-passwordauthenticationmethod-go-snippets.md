---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebf7c6805aa3c200cb39a41033e81209a4285610
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328394"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

passwordAuthenticationMethodId := "passwordAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordMethodsById(&passwordAuthenticationMethodId).Get()


```