---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff111c8afcc2c2b4bf52cf5cd608cf88b20843dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```