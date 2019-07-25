---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 564a460f582775cbd86de53be9379281ed7ebdbe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895354"
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