---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ba312a5d87d8cab990c0da8c57bcabeb91d7c55
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sets = await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"].Sets
    .Request()
    .GetAsync();

```