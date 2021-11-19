---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e8cc20419e0b182289fa9548d7ec62f976dc1ce
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().DailyPrintUsageByUser().Get(options)


```