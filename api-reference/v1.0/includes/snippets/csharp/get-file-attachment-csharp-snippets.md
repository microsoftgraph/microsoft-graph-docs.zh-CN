---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e350960691e1e3069ecf9fb1717daa13b99e7a2c
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["{id}"].Attachments["{id}"]
    .Request()
    .GetAsync();

```