---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 893d9bee96de218d88ceb4f9ce7c4c16c8d64f9173ba323f1120dbceb0b2ea67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoles = await graphClient.PrivilegedRoles
    .Request()
    .GetAsync();

```