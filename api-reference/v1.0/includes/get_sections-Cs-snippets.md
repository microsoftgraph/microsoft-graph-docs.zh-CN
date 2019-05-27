---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0cfb221772fd5ce974ee25901e2520f2c55c1975
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .GetAsync();

```