---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31da8ccfa96c371faa677bdb4ab19a73280dc61d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityCounts('D7')
    .Request()
    .GetAsync();

```