---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49b4afa854f99e66fb3a84216a8570ce0130876e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329007"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Print().Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get()


```