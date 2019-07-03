---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d274dee65cd5f5821bd186b1926bde3270c35aaf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityCounts = await graphClient.Reports.GetYammerGroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```