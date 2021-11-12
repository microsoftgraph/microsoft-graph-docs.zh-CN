---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d9d9d3f281fa02170417217aa594f0e0d7b9a58a14b29287f97cdd73f4167bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378271"
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