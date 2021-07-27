---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d1d60a06267e92a78a3fec02f7f9beb8c371ed
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .GetAsync();

```