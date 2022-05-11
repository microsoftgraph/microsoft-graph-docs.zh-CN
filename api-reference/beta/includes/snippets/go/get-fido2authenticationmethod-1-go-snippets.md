---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7efd121836b2b8e148ba7f7065445a71089d751f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329189"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
result, err := graphClient.Me().Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Get()


```