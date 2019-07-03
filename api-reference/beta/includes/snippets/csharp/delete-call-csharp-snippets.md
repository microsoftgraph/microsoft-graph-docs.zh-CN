---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 881ec7bac57269dbf90029c04bc7ea76988cf56c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"]
    .Request()
    .DeleteAsync();

```