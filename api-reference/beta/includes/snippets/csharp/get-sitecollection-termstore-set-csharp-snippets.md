---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 721698c2e5cd09a95ee638ed8eedd0d00f375630
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"]
    .Request()
    .GetAsync();

```