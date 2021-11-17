---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2319f79e51cc85320276e92b1990e67dc7690f2b942ae1bd0e3ba90a90d7098f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378606"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods["{temporaryAccessPassAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```