---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d687272499313f35fcb57af76c310b91607d2418445b43b3072b9d7e07e40867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .GetAsync();

```