---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ad48b76ad1ea9205ba92a325b5b9e8b66e1fda6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327859"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ContinuousAccessEvaluationPolicy().Get()


```