---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3dc89c1654721a947edabe3cedf509b543eccfd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessActivityCounts('D7')
    .Request()
    .GetAsync();

```