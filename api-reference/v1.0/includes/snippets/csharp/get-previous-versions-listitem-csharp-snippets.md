---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84a3630a98d9fe2dc3a8497154ef9e56e22885b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Versions
    .Request()
    .GetAsync();

```