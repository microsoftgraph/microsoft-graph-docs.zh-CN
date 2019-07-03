---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c5313ea7cc551c3d7c14fd02b011460ae45a3fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466816"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActiveUserCounts('D7')
    .Request()
    .GetAsync();

```