---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09d143dbf9c7b14c2180817bb8b2dbc50284feb0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Send()
    .Request()
    .PostAsync();

```