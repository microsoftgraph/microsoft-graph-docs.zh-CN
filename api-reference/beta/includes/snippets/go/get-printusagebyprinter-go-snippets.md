---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d13b4fee010a60376a1b03a395230fc525fe95f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByPrinterId := "printUsageByPrinter-id"
result, err := graphClient.Print().Reports().DailyPrintUsageByPrinterById(&printUsageByPrinterId).Get()


```