---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62392cbfdba39493a4ce85a0a6c31281f5e742292bbf48d7b930eaa846f38dce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request()
    .GetAsync();

```