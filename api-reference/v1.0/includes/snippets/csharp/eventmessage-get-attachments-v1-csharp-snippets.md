---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff29bbad94daeb381a85f2507e65ef80eef93bf5
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .GetAsync();

```