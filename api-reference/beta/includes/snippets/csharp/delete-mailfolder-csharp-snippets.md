---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c3502e6d39bcb3d0387f52d6abcc4d1a02d589c8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .DeleteAsync();

```