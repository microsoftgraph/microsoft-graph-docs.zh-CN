---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 886da2bf000935b475cbfba040164a3fe3d28ef3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplate = await graphClient.ApplicationTemplates["{id}"]
    .Request()
    .GetAsync();

```