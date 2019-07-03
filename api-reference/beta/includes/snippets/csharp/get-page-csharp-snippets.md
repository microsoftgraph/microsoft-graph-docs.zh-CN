---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d93fa7cb5282aa6e0ad2ae4b4fb9cf925828b375
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{page-id}"]
    .Request()
    .GetAsync();

```