---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcbc062cb8cdbee6409ec23c3503e4b147532624
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Sections
    .Request()
    .GetAsync();

```