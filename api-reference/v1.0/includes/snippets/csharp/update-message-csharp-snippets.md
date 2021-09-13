---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b3987a2e7645780f5eb4c4454a5d6b77fd86aa01cf5b3eb93b246ec6e266d62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "subject-value",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    InferenceClassification = InferenceClassificationType.Other
};

await graphClient.Me.Messages["{message-id}"]
    .Request()
    .UpdateAsync(message);

```