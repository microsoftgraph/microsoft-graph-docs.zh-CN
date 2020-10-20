---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f01c5c796f23d3c1787aa1de246614d305678c8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredOwners = await graphClient.Devices["{id}"].RegisteredOwners
    .Request()
    .GetAsync();

```