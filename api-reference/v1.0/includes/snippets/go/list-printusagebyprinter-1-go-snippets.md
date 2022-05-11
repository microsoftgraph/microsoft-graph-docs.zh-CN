---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 995d84f582663355a0bf7c49c6f3c34fdddc170a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().DailyPrintUsageByPrinter().Get()


```