---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d21245cb1a4a8361abda69ebeb557da83c139f60
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411997"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
result, err := graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Delete(nil)


```