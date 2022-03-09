---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db41d0c0df2929664ecbe7332664ea1a7605ba5d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395648"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Print().Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get(nil)


```