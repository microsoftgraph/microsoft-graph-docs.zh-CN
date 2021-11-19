---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 467a3018428cd2fcdd299ee9183992f5383c7aa2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085571"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Delete(options)


```