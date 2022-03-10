---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 022657bb8a528475a512eeda04b32c721adb3397
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Delete(nil)


```