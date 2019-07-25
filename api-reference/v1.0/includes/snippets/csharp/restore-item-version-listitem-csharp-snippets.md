---
description: 自动生成的文件。 不修改
ms.openlocfilehash: caf21267de7add61c2fc0d560f26bdeab9758c36
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions["{version-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```