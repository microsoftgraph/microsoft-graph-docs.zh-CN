---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f92ad0c29a5e78d770b15457768a164fb86efd11
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = await graphClient.Me.Outlook.MasterCategories["{outlookCategory-id}"]
    .Request()
    .GetAsync();

```