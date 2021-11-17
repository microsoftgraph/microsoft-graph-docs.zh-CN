---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70ba8899c780c67f2826be8d149918bd3fe38116
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
windowsHelloForBusinessAuthenticationMethodId := "windowsHelloForBusinessAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethodsById(&windowsHelloForBusinessAuthenticationMethodId).Get(options)


```