---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba90c43045fa747cd0806eb476dd192d385c8c098645c91b6fb44558d0ff1353
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMemberOf = await graphClient.Me.ScopedRoleMemberOf
    .Request()
    .GetAsync();

```