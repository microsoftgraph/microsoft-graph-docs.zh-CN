---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29522765be4bbe5b7c35f46a2a0ffa7ca38f3f2c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var inferenceClassificationOverride = new InferenceClassificationOverride
{
    ClassifyAs = InferenceClassificationType.Focused,
    SenderEmailAddress = new EmailAddress
    {
        Name = "Samantha Booth",
        Address = "samanthab@adatum.onmicrosoft.com"
    }
};

await graphClient.Me.InferenceClassification.Overrides
    .Request()
    .AddAsync(inferenceClassificationOverride);

```