---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ad5ecfad41d37b64a55cbb2eb2438a00877d2a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{id}"]
    .Request()
    .GetAsync();

```