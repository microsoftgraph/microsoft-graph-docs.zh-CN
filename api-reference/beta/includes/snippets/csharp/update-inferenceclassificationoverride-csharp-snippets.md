---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4378a64828da20e06b630a295a8b0c28a6a26a2e75eed409d26ac756a1283db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163409"
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