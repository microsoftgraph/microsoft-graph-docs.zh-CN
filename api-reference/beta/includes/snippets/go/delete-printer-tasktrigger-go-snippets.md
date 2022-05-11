---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 759e5f8ad5e95ba3c9703c84e8680da69f843835
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327437"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Delete()


```