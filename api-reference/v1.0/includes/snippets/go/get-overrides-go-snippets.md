---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49cf86ba4ca41e0c4ff5359e31a674b2d6ddd89e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325723"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InferenceClassification().Overrides().Get()


```