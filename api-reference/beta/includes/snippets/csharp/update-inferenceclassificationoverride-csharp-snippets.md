---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2a187215b6c350080790cd883cef71d46d33b51
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var inferenceClassificationOverride = new InferenceClassificationOverride
{
    ClassifyAs = InferenceClassificationType.Focused
};

await graphClient.Me.InferenceClassification.Overrides["{inferenceClassificationOverride-id}"]
    .Request()
    .UpdateAsync(inferenceClassificationOverride);

```