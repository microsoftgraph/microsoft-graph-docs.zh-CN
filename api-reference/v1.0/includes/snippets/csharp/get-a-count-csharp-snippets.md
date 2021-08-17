---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b0291972845bb717865d129ea25336b84edc862
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName,'A')")
    .OrderBy("displayName")
    .Top(1)
    .GetAsync();

```