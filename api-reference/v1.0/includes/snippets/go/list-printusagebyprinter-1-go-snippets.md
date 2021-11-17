---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9917d14c7360dc6d0cf1d8c8a0eec30facc3543c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992507"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Reports().DailyPrintUsageByPrinter().Get(options)


```