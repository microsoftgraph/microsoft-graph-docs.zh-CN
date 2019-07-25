---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de0e347856abdac5711bdf4d63388b1d003a4d8c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Sites["{siteId}"].Drives
    .Request()
    .GetAsync();

```