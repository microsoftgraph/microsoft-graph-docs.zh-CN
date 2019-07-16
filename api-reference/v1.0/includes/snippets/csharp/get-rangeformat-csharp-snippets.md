---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82bb840784bb1674f3456541a91a4389b2b68b98
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format
    .Request()
    .GetAsync();

```