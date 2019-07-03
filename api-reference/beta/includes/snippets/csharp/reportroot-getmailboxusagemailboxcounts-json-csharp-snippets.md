---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 79a7a6b1f29e5b17131b86fcd787e60ce09b15ec
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageMailboxCounts = await graphClient.Reports.GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```