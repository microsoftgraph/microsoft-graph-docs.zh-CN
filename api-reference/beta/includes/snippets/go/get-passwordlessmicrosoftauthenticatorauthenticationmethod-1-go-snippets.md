---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a5df34a0797aad19377913b861814920ef874c6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

passwordlessMicrosoftAuthenticatorAuthenticationMethodId := "passwordlessMicrosoftAuthenticatorAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordlessMicrosoftAuthenticatorMethodsById(&passwordlessMicrosoftAuthenticatorAuthenticationMethodId).Get(options)


```