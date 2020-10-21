---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b81c390c250d4f1105535bdb7eb407bd70a1d030
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{id}"]
    .Request()
    .GetAsync();

```