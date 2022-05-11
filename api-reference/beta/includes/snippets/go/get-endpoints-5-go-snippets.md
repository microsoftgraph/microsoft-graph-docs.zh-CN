---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d064194523838e373ca8a80bb7b2e82c4519ca8e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326668"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().MonthlyPrintUsageByPrinter().Get()


```