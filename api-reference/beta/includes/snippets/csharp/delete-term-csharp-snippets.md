---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19d9af3d324fdbc234aabe19cb15b5421a9cd92
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{setId}"].Terms["{termId}"]
    .Request()
    .DeleteAsync();

```