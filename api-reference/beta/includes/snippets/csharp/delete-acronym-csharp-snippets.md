---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5e42675f212b818da7978969473af72a1fcd60f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Search.Acronyms["{search.acronym-id}"]
    .Request()
    .DeleteAsync();

```