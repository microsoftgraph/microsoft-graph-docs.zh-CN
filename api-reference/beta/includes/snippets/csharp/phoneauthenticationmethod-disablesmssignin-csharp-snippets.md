---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3901701144444628f7b44414a5c0432b85097a91bb86a18ca0065a69978aa7d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .DisableSmsSignIn()
    .Request()
    .PostAsync();

```