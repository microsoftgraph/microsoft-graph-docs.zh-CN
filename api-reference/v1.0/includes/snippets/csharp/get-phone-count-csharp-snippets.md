---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d1d60a06267e92a78a3fec02f7f9beb8c371ed
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .GetAsync();

```