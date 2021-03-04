---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f3d7e3f2e19ce748dc952f5dc6bc19f9369afa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445027"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```