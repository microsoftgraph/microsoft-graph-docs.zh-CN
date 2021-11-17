---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7097b94d571f5db1670499090cc2c36c2089dbd81141a0653fdc260c50a696d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Unfavorite(messageIds)
    .Request()
    .PostAsync();

```