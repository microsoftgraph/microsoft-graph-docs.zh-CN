---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3516066cecbd205d52f933ec8b4a91e3cb8fbd4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "description-value",
    DisplayName = "displayName-value",
    GroupTypes = new List<String>()
    {
        "groupTypes-value"
    },
    Mail = "mail-value",
    MailEnabled = true,
    MailNickname = "mailNickname-value"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```