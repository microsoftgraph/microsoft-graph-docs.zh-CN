---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c5ed53458a48b04fc1543c7fe146049cfe82afc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Protection
    .Request()
    .GetAsync();

```