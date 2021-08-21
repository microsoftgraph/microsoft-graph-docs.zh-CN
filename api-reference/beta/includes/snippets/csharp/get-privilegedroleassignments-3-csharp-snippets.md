---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 580a1f2c9546fc1121d86c8fe32609861e21dde3ca5e06f92447e7ad024f1dc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .Filter("isElevated eq true and expirationDateTime eq null")
    .GetAsync();

```