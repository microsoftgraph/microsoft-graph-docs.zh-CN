---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c18a3e617e89748b6c11d1b8de81e664d6a8077e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["{id}"].Events
    .Request()
    .GetAsync();

```