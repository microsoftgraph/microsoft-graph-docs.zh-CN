---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d1e9c8149496e2707d426f0fa68ac28c442873fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageDetail("D7")
    .Request()
    .GetAsync();

```