---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 015a6ad1ddfc1ba98659704c051e71ef0a863e9435079b9bcbfd9322ba021061
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')")
    .Select("displayName,id")
    .GetAsync();

```