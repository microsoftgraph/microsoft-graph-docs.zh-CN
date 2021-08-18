---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1a8995656b4249cf20e8cfab62595f2a29387ce2d348cfc7c304c0d95ff17c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("startswith(displayName,'Eric')")
    .Select("displayName,signInActivity")
    .GetAsync();

```