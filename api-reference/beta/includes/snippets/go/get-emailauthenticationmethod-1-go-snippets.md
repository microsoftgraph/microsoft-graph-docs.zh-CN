---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 181d16e0d9a6d001bb963873ace17f4f6bc8bd64
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

emailAuthenticationMethodId := "emailAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().EmailMethodsById(&emailAuthenticationMethodId).Get(options)


```