---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7cea20cb1472738691fd730d4bd0ebcf3a56aa62
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request()
    .GetAsync();

```