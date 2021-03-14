---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84b6157956af55b944ef7c1cf099a3b35e599316
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .Select("displayName")
    .GetAsync();

```