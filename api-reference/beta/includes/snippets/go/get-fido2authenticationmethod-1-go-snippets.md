---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5106a273408f222789cd64b925bfc228a4b4571
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
result, err := graphClient.Me().Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Get(options)


```