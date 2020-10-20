---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9733a179d2bdc2c2d3dcd0ecec4fa86db5486b68
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .RevokeSignInSessions()
    .Request()
    .PostAsync();

```