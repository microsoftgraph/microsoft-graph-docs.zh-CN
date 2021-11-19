---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17253d74e95f5813e6445dc5cd25d69094fe4048
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ContinuousAccessEvaluationPolicy().Get(options)


```