---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35d0af3bfa42f85c0b5ab350895a99f7b49d6ab9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{id}"].Manager
    .Request()
    .GetAsync();

```