---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b803cacef838d3485ef11fc8dd3bef091c4f7d9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997644"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Get(options)


```