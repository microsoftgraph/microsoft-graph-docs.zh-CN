---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c54a9e60c55aee9752d8173e3c1557071fd4da49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .GetAsync();

```