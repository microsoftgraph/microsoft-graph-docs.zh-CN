---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5b0171d39c467e48863cb5e2736fa61f5a43149
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091515"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().MonthlyPrintUsageByUser().Get(options)


```