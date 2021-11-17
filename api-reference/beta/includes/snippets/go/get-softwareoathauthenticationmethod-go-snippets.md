---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f41423f9f438840f3bc9fa6e3237c22f29c1552
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020376"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Get(options)


```