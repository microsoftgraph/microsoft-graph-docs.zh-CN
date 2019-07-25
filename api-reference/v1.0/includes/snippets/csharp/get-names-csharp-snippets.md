---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfcdf0f03ada674e169315da651e80e5ca10a938
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711226"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .Request()
    .GetAsync();

```