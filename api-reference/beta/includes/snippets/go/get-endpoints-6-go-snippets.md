---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7309f1d53f38e28383b58320f3a840c4af7e0c58
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397335"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().MonthlyPrintUsageByUser().Get(nil)


```