---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 864726633d78e89a85757934fa6e30a66823afd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Notebooks["{notebook-id}"].Sections
    .Request()
    .GetAsync();

```