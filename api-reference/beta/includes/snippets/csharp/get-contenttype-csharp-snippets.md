---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c36c72f64921b92d255ec68c2738bb00608960e94c911d3001db6d42a6da1aa6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Request()
    .GetAsync();

```