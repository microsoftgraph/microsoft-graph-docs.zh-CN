---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce790aa689bc474f734c8258db06c07ac852c17b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102468"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

passwordAuthenticationMethodId := "passwordAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PasswordMethodsById(&passwordAuthenticationMethodId).Get(options)


```