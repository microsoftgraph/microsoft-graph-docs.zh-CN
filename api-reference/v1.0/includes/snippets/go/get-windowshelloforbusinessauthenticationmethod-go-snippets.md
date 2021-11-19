---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78f9ab4af8c40385277a5af6e6a458c3292c7fad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088965"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
windowsHelloForBusinessAuthenticationMethodId := "windowsHelloForBusinessAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethodsById(&windowsHelloForBusinessAuthenticationMethodId).Get(options)


```