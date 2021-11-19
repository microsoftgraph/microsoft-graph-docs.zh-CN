---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f479e20bdec2acfdf1e423174a43aa0d0711dfe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().MonthlyPrintUsageByPrinter().Get(options)


```