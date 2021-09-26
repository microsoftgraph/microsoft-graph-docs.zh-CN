---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29dff7ad424e336dfec2ab5c83ec7e39c1b2cd7bc9bd762b6bc8ff31b41ff26a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .GetAsync();

```