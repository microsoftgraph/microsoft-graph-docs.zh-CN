---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32b84e687f8d114f779ec73df980f9bb6abc44996f785ee575d78956519dbbed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Summary
    .Request()
    .GetAsync();

```