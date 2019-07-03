---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c705ab4914cbf229f6a1e41d6a3fc0df3d52c48
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["{id}"]
    .Request()
    .GetAsync();

```