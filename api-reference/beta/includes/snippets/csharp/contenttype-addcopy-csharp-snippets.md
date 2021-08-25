---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73d41ad8f00d292b4ff115987c8557eb3bb6caf5e6330018119e5361cb0c2f38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopy(contentType)
    .Request()
    .PostAsync();

```