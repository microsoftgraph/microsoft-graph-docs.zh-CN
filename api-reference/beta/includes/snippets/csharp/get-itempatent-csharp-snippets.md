---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6231b8fdc16c4f0bdeb9c52fb8d04495933fb03e08aa9a54f7a402ad2d931f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPatent = await graphClient.Me.Profile.Patents["{itemPatent-id}"]
    .Request()
    .GetAsync();

```