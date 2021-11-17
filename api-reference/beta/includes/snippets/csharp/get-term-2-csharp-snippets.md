---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 796cfb9bce8a800e563881c1a3ea854fbdaddd87737ec23deaad4bda85810a89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279622"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.TermStore.Sets["{termStore.set-id}"].Children
    .Request()
    .GetAsync();

```