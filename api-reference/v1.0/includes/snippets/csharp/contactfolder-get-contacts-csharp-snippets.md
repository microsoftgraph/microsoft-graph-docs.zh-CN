---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3ea2d6c17b17bea790520eb3fa9232394a547b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.ContactFolders["{id}"].Contacts
    .Request()
    .GetAsync();

```