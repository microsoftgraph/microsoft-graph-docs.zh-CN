---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c9ef9e2b30737c0fd51ec712312252774e0d12b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessActivityCounts('D7')
    .Request()
    .GetAsync();

```