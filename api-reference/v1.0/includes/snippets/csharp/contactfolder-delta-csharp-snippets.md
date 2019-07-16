---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cebc9f1372097ca89c92f16edc9e9061cca9f3c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```