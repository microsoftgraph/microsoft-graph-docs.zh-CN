---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 11e41490096e441a64cffcb98e9c3579344a5de6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = new Notebook
{
    DisplayName = "Notebook name"
};

await graphClient.Me.Onenote.Notebooks
    .Request()
    .AddAsync(notebook);

```