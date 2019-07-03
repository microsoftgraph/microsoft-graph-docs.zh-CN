---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61c2ac2ef751b2ac5eaa9833b12f8e51ca068aeb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessParticipantActivityCounts('D7')
    .Request()
    .GetAsync();

```