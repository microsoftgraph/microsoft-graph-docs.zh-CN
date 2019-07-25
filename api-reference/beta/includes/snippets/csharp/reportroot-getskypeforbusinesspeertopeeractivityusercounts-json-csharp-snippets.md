---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 23f0d1692c33596fe2dd4bbbb7ca643f92aec56d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```