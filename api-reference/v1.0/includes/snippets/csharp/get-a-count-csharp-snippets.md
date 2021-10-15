---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b0291972845bb717865d129ea25336b84edc862
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "59766234"
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