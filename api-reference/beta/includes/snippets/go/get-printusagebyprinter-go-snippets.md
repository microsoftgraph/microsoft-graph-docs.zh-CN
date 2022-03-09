---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 092e3533cea9a0165b0800c1ac143dd0abfdb468
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397181"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByPrinterId := "printUsageByPrinter-id"
result, err := graphClient.Print().Reports().DailyPrintUsageByPrinterById(&printUsageByPrinterId).Get(nil)


```