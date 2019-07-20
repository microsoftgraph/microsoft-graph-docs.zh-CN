---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 89658912c0db797e2c89fb318ba8465b1629b241
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageDetail = await graphClient.Reports.GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```