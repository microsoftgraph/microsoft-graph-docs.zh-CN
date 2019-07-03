---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcedae9c632ef0d55e7bfcad469cb9273eba418c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519992"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityGroupCounts = await graphClient.Reports.GetOffice365GroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```