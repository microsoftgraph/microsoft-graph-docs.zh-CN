---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc1f98b2fdd74e6485f9e56718d70057e6b6a314
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412676"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemEmailId := "itemEmail-id"
result, err := graphClient.Me().Profile().EmailsById(&itemEmailId).Delete(nil)


```