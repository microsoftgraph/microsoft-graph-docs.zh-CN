---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff77af856d954285f6285f9b42033191122c0fc3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Connectors().Get(options)


```