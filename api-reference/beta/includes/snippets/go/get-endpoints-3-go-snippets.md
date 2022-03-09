---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52e12a3a6d1cc828493517eba9ef8ab3ae23e445
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().DailyPrintUsageByPrinter().Get(nil)


```