---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 15c62d0c9d84dcee968247047b40dc92e3f4e0e6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRecentNotebooks = await graphClient.Me.Onenote.Notebooks
    .GetRecentNotebooks(true)
    .Request()
    .GetAsync();

```