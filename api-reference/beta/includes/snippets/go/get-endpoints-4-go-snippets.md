---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe4f7e29a9397bbdb8cb926b3c5438b6c4b101a9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396250"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().DailyPrintUsageByUser().Get(nil)


```