---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c730f247acd23c804984a339bead51b1d3d6b117
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288159"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Delete(nil)


```