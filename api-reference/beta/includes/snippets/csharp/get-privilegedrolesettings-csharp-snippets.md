---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d196a7c89b6df73a4d67c48bd3eb56c12b6bba318350c3ce0c657837e3f61624
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Settings
    .Request()
    .GetAsync();

```