---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e91029a80fcafa7e49391ac50ac6dc5d6e269a5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326483"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

authenticationMethodId := "authenticationMethod-id"
result, err := graphClient.Me().Authentication().MethodsById(&authenticationMethodId).Get()


```