---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faa410a93c44135a07f54d4f19f54a206873f19e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Get()


```