---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b42a77581db41701eb4bbc7ecf0cfb1cb644c72b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var points = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"].Points
    .Request()
    .GetAsync();

```