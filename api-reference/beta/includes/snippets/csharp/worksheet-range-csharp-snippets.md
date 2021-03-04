---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e52d092fe52d55e53f9693f542f1d8273613ed6a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range()
    .Request()
    .GetAsync();

```