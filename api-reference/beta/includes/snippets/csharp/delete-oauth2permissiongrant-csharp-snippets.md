---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4704bcf05f8ec173451f0b4d7d66dbef23b7be35
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .DeleteAsync();

```