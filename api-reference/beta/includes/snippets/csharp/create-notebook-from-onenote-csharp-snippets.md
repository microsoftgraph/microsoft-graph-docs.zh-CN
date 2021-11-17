---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 410effc6d117e28701452608f15e8845683e5b431b815d145819dc17481c165e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = new Notebook
{
    DisplayName = "My Private notebook"
};

await graphClient.Me.Onenote.Notebooks
    .Request()
    .AddAsync(notebook);

```