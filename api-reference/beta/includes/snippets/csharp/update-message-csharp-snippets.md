---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a963d8fc869aacfde5ff9d1bc390dd11acec3f6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479856"
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

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```