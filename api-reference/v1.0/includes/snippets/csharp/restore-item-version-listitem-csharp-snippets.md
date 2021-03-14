---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583aea606d66ec90595b9d653a9d26d1c6a39736
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Versions["{listItemVersion-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```