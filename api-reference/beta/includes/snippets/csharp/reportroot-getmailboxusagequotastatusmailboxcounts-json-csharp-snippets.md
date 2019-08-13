---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31100aeebdd22a3dd85f5d82297245e9e6536b48
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageQuotaStatusMailboxCounts = await graphClient.Reports
    .GetMailboxUsageQuotaStatusMailboxCounts("D7")
    .Request()
    .GetAsync();

```