---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c67946d87c27fc972e59c5da871a23eabd2e9d8f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091185"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get(options)


```