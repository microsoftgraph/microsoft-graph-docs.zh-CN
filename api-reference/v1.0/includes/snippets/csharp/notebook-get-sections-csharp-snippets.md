---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5de4df6ea5843a837df3ab1d7383384ee5713ea4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Notebooks["{id}"].Sections
    .Request()
    .GetAsync();

```