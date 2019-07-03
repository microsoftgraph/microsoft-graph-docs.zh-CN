---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 441bd7dc497bd2af2ae48b1d083109bb43f0c98f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookApplication = await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Request()
    .GetAsync();

```