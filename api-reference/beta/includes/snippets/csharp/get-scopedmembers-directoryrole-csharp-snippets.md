---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55a6388a33c0c5d7687550fccbc2d7e09fb3d4e0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedMembers = await graphClient.DirectoryRoles["{id}"].ScopedMembers
    .Request()
    .GetAsync();

```