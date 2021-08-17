---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d8452c0995c17c1adf44697607599dc2d962d925c1489571ef7aae9fb035cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .GetAsync();

```