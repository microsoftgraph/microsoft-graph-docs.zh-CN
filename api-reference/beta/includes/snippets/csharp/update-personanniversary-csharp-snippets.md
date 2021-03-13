---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f34a86f5337f062e1806cd861573a3e8a8c854f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
    AllowedAudiences = AllowedAudiences.Contacts
};

await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .UpdateAsync(personAnnualEvent);

```