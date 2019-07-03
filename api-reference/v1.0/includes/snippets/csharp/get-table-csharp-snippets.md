---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54a5a70ea71a3cb83870a2c4f610b019ec109bf3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Request()
    .GetAsync();

```