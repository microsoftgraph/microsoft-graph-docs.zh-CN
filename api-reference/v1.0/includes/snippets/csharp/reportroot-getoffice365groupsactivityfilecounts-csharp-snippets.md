---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a446c19fcbcf6ea95976171668cf06129ed32069
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts('D7')
    .Request()
    .GetAsync();

```