---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 127a1df3a839896798bfc78ec370661d5ce6d64d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = new ItemEmail
{
    DisplayName = "Business Email",
    Type = EmailType.Work
};

await graphClient.Users["{user-id}"].Profile.Emails["{itemEmail-id}"]
    .Request()
    .UpdateAsync(itemEmail);

```