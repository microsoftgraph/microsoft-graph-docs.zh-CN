---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1c0d24514a2490fc8eb9b7dcdbe9ca693c752c0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .Request()
    .GetAsync();

```