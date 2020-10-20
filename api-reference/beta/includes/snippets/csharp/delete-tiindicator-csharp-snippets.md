---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ff62041649bb1ebf8589c4686f85c592961b7de
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .DeleteAsync();

```