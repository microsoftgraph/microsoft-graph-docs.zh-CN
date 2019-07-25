---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ad5ecfad41d37b64a55cbb2eb2438a00877d2a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{id}"]
    .Request()
    .GetAsync();

```