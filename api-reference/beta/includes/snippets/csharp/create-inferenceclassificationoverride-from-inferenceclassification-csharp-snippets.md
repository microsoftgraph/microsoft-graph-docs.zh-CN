---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecace088bb417e86399905882757ac6b68888f8169d55969e5ab59d7ff87c295
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333024"
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