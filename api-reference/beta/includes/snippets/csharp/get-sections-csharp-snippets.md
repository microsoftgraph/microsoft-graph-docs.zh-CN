---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0cfb221772fd5ce974ee25901e2520f2c55c1975
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .GetAsync();

```