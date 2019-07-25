---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a37fccafdc8707fd5635da7b2cfb97f9fe54440b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .RefreshSession(this)
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```