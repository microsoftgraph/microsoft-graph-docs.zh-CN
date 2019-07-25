---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb345d8ac1c25ff29197cb7646da7af78261c627
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Me.DirectReports
    .Request()
    .GetAsync();

```