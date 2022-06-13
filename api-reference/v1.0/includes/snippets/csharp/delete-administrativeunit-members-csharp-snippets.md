---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f38c135df593815b7d1891a387f35ddb3b1a918
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040871"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].Members["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```