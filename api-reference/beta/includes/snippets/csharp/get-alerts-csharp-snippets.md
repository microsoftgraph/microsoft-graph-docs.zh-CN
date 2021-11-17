---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fbd3ed6e34a59289df6d9f75253de9738c1487acb773e27d06f317a16f11f98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts
    .Request()
    .GetAsync();

```