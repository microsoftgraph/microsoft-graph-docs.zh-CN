---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e7159a00245598cb47fb92f9b670f9b16560b3565f3b90198c84f88fd1247f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.IdentityProviders
    .Request()
    .GetAsync();

```