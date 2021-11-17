---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 783f18d960de61c5b8bc0bb0a721c6ac36b7fc24
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().MicrosoftAuthenticatorMethods().Get(options)


```