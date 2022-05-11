---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dd066160a8241cda3f78113f044da9710055491
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypeId = "0x0101";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopyFromContentTypeHub(contentTypeId)
    .Request()
    .PostAsync();

```