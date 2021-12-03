---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4491681ebd9bea80f5a3001d1d437a7c18363db5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Delete(nil)


```