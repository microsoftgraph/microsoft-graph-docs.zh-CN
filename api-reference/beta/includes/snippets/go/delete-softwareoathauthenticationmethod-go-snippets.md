---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c8f3f582d6c2921cb43281cf3d4f7ff6d638aa3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Delete(nil)


```