---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edb96bcb6e68582b65bb0730d09795187a7339118c7884507842e930ce674019
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```