---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1cd415e3f73f1408a85fa425804b1bf923a31fe2d5b2391c33025fa15bac841
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .EnableSmsSignIn()
    .Request()
    .PostAsync();

```