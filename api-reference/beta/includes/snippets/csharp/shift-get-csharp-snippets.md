---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c9d17e1931bcfe80229c5ca8fe641d2009ba139
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .GetAsync();

```