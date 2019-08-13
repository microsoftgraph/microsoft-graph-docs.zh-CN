---
description: 自动生成的文件。 不修改
ms.openlocfilehash: adf16957110d5bed55cdd51d5004e5b80dfac323
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308671"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageMailboxCounts = await graphClient.Reports
    .GetMailboxUsageMailboxCounts("D7")
    .Request()
    .GetAsync();

```