---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12d9a5707e6c6c23d76417f6f9dfc0e278a786b0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Users["{idOrUserPrincipalName}"].Drive
    .Request()
    .GetAsync();

```