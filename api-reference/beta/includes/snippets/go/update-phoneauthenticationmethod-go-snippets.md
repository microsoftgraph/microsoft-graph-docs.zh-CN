---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 147c1b79024bb9310592eff154277815db679e79
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Put(options)


```