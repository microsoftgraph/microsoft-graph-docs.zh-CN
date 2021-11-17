---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b26c693b7de76f9d7fad0ccd563b34594cd9a4e5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Reports().MonthlyPrintUsageByUser().Get(options)


```