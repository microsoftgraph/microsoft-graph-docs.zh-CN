---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e58103ef2faea27c6d14683af0b356758232fd30
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageMailboxCounts("D7")
    .Request()
    .GetAsync();

```