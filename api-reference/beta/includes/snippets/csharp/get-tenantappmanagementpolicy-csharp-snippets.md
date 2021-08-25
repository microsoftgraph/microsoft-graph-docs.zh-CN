---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e894d6fdeb5703b5a5764476e9b3bdf883539a43
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantAppManagementPolicy = await graphClient.Policies.DefaultAppManagementPolicy
    .Request()
    .GetAsync();

```