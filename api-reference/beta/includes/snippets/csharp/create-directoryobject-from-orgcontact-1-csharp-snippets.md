---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb209ac769a2b9387efd749534738868e88e47fd4f17890168b7ae6caf6e2ade
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directoryObject", "{}"}
    }
};

await graphClient.Contacts["{orgContact-id}"].DirectReports
    .Request()
    .AddAsync(directoryObject);

```