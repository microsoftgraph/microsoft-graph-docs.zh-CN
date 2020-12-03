---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 731d2eed800b134c9ca598be8760f0afbb64c73f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{id|userPrincipalName}"].Manager
    .Request()
    .GetAsync();

```