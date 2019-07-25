---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a82bea549d8b263827d5eec39206aaa5d0edd992
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageStorage = await graphClient.Reports
    .GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```