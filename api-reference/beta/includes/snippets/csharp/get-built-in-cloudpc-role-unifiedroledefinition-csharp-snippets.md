---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3759b6ed24d5d3d3166a72e1dbc991ff54be1f2c71fbeaad07bd6ffef64e3c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.CloudPC.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .GetAsync();

```