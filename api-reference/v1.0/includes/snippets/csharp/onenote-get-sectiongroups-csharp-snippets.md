---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fd4e873873491ea2465fa029e505145f389e5646
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups
    .Request()
    .GetAsync();

```