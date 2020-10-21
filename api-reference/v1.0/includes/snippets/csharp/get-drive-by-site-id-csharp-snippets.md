---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdcafc495087b78ccc156b4fe25fdcca7b97636d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{siteId}"].Drive
    .Request()
    .GetAsync();

```