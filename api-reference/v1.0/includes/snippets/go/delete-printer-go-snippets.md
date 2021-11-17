---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2dd3e18891977c84951549b61afbdc016bac336
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003526"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).Delete(options)


```