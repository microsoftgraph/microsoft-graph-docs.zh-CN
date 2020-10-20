---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4002b673791aebe1f85b7d5aa36c1e7d3f77ca46
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directoryroles["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```