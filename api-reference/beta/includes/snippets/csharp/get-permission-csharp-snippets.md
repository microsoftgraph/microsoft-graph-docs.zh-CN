---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16907d10164c641d0cfd914c49767dc990e4b8a109f884e5445104cfc3cf38aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .GetAsync();

```