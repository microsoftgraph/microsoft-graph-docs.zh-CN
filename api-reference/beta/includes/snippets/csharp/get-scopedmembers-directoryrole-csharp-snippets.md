---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 55a6388a33c0c5d7687550fccbc2d7e09fb3d4e0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedMembers = await graphClient.DirectoryRoles["{id}"].ScopedMembers
    .Request()
    .GetAsync();

```