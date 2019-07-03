---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 564a460f582775cbd86de53be9379281ed7ebdbe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.EmailAddresses 
             })
    .GetAsync();

```