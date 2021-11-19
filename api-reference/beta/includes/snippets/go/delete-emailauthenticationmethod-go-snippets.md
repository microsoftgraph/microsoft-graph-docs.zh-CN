---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a54d0cbb55a8b3946488dc9c61c580974de1755
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
emailAuthenticationMethodId := "emailAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().EmailMethodsById(&emailAuthenticationMethodId).Delete(options)


```