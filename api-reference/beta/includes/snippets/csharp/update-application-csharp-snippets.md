---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e95f0a8f46950f3d2ccdf39c0bc3ad4f75afd7d01e2ee23bf977346acb4c438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "New display name"
};

await graphClient.Applications["{application-id}"]
    .Request()
    .UpdateAsync(application);

```