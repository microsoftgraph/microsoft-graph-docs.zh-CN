---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfcdf0f03ada674e169315da651e80e5ca10a938
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .Request()
    .GetAsync();

```