---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d1d60a06267e92a78a3fec02f7f9beb8c371ed
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .GetAsync();

```