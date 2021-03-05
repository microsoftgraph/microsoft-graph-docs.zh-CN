---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4751453c87f44b3dbfb69e74a46fef94a0c59582
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.TemporaryAccessPassMethods["{id}"]
    .Request()
    .DeleteAsync();

```