---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01c9e75d7e1d5c3718499256a7b159391cec4c8e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287853"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ContinuousAccessEvaluationPolicy().Get(nil)


```