---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75e2f80d99e3eb082dd2aac4d2538fdc25dfaa7a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092494"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Security().Cases().EdiscoveryCases().Get()


```