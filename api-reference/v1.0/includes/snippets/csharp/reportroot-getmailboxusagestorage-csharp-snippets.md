---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba4974468c1661b03b8baefe2e46c106fb50d2e4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```