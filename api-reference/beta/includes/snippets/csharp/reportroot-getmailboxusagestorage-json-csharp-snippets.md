---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 294e70633fbc069a9328641d9bd9b73b7d48c992
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageStorage = await graphClient.Reports
    .GetMailboxUsageStorage("D7")
    .Request()
    .GetAsync();

```