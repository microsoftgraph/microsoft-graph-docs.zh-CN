---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb6b42f48a9ecfd6633ab963d23a584b78a7c86c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Delete(nil)


```