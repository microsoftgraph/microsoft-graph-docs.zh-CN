---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f6c8e8136cb0a281f72879d63dec2a6c663513bff814c84f819ef581aea221
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{sitePage-id}"]
    .Request()
    .GetAsync();

```