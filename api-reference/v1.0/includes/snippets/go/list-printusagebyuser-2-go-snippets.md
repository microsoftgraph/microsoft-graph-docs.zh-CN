---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e4d29158f57a1f6386e4654b1f214c0f4effe6b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326225"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().MonthlyPrintUsageByUser().Get()


```