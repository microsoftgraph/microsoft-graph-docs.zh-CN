---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fa9e470b6034e7efefb0c4fdf7cae9e403ececf
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
};

await graphClient.ServicePrincipals["{id}"]
    .CheckMemberObjects(ids)
    .Request()
    .PostAsync();

```