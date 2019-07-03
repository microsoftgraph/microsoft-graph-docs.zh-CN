---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 89658912c0db797e2c89fb318ba8465b1629b241
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499661"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageDetail = await graphClient.Reports.GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```