---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7072ee5337e67f6bd535f05371b256b3a5928776ec6e373ec853c9017fbd2ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .MarkRead(messageIds)
    .Request()
    .PostAsync();

```