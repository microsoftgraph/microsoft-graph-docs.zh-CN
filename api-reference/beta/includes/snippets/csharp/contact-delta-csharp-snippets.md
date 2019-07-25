---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef52b73b8435911277e8e9231e46167693e628a6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{id}"].Contacts
    .Delta()
    .Request()
    .Select( e => new {
             e.DisplayName 
             })
    .GetAsync();

```