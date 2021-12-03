---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6ca80dfdf37b5e2693435c7b1adb79686bfbffc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287682"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
result, err := graphClient.Me().Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Get(nil)


```