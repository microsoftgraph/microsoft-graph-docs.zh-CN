---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a975f5a2ab7f28e3069d9ad5d7b224a80e0fffc2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992479"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Reports().MonthlyPrintUsageByPrinter().Get(options)


```