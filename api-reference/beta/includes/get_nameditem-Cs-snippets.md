---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 054336833d11d1d6e5ac5cfadb5a55f2dc4b6b7b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Request()
    .GetAsync();

```