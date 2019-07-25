---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 886369656b226e5d07a2d6744fe4687ed6f0c502
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "Sheet1!A1:D5";

var hasHeaders = true;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Add(address,hasHeaders)
    .Request()
    .PostAsync();

```