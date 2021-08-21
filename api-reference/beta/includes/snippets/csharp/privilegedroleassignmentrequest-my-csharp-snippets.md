---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6081ee015803770b824990e7c8454ab8307c7f611d96bb944a4fd68d3afb7d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignmentRequests
    .My()
    .Request()
    .GetAsync();

```