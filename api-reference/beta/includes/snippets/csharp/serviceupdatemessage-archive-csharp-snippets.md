---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c1e28f42d83dd86a18fe9bd2b1b733fca3c624a9b5fb28ccb062e38cb196661
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Archive(messageIds)
    .Request()
    .PostAsync();

```