---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0ff7056abec2f7b835f3bf1ba5cd06de8dd6ce3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessOrganizerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```