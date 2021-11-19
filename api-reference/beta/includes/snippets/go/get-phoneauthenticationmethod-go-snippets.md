---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50444a63bbd7d3c71c046388a898bf3ee2ed40de
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101393"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Get(options)


```