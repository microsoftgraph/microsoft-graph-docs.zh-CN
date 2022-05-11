---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71d5c33d0dd7685c8a44160a027beec28bf4fa57
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327977"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
microsoftAuthenticatorAuthenticationMethodId := "microsoftAuthenticatorAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().MicrosoftAuthenticatorMethodsById(&microsoftAuthenticatorAuthenticationMethodId).Get()


```