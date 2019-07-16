---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0c1f55373473cdc94cd9d1265494b32909e6df3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .DeleteAsync();

```