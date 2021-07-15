---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 213a21c9185ed70b9466e02efa93c444b62913f2
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Contoso Life v2.0",
    DisplayName = "Contoso Life Renewed"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```