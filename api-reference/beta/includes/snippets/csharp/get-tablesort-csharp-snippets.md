---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f8380ff93709a01eec793180b5064684a36e935
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableSort = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Request()
    .GetAsync();

```