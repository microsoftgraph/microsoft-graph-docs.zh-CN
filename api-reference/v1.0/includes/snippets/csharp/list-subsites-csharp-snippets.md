---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d0bfb7d6ee1465c79559ffcecccb736c6d0a9d0e02cd2e712500af6f78c640d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites["{site-id}"].Sites
    .Request()
    .GetAsync();

```