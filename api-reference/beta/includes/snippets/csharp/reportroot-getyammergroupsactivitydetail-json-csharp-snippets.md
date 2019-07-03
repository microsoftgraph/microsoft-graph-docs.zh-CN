---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f39fa5a476d479c211249d9eb2c85bb1ceef48a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityDetail = await graphClient.Reports.GetYammerGroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```