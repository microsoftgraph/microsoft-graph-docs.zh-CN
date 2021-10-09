---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6338936444751d4df802a5d2af6931305f684580d6d17d051fdec52e7b8023b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    RoleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```