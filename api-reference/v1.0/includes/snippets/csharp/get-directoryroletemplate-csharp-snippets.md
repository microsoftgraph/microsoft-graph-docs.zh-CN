---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ad5ecfad41d37b64a55cbb2eb2438a00877d2a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468040"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{id}"]
    .Request()
    .GetAsync();

```