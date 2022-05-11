---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0edfc0f5f3d982c91ed81f75c1ec77522f5ae597
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().MonthlyPrintUsageByUser().Get()


```