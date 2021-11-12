---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdce56a9a5d163bf7c0f5bcb78f309a953b1b0f443ced0a51bfc7eb5aa28503c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = new Microsoft.Graph.TermStore.Set
{
    Description = "mySet"
};

await graphClient.TermStore.Sets["{termStore.set-id}"]
    .Request()
    .UpdateAsync(set);

```