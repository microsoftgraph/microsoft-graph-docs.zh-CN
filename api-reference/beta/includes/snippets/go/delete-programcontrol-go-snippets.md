---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daadac51b7182ff6835bd265c5c0a5f2a5b6c233
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396320"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programControlId := "programControl-id"
result, err := graphClient.ProgramControlsById(&programControlId).Delete(nil)


```