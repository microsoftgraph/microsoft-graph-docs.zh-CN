---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed7068b512730d0e3cfa02f40180093076882f7a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Get(nil)


```