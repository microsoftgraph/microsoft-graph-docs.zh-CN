---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1286293c0d020f9965f0253719919a0ac5db620f2d337b71bf4740493caf279
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Versions["{listItemVersion-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```