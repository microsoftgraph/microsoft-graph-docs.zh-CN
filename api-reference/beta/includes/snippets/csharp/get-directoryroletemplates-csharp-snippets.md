---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 277c00a003486e33a62f8af21ffea72f8f45fa29
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713326"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplates = await graphClient.DirectoryRoleTemplates
    .Request()
    .GetAsync();

```