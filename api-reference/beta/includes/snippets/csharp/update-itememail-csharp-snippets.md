---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc90169a6ea3258c732958c500abcd681cdd208a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = new ItemEmail
{
    Address = "address-value",
    DisplayName = "displayName-value",
    Type = EmailType.Unknown
};

await graphClient.Me.Profile.Emails["{id}"]
    .Request()
    .UpdateAsync(itemEmail);

```