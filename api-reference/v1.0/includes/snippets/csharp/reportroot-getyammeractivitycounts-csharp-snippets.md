---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6614dc26bd31fdec5eedf4e381f741bde6e958e3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```