---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d94bb860a5881952b55fc6b643511e3fc7d0f77
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Shares().Get(options)


```