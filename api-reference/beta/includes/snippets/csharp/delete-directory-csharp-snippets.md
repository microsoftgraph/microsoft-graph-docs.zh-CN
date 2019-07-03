---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4cd88a0695a1ac3ef4ad981dc68bb26e1941d671
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["46cc6179-19d0-473e-97ad-6ff84347bbbb"]
    .Request()
    .DeleteAsync();

```