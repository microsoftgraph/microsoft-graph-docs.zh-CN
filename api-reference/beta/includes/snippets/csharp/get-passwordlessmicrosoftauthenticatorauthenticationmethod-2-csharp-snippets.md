---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6986f3cf941dee7f7fd4b81598d804b7811ac7d07586ba6a54e151a2151e7ecd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordlessMicrosoftAuthenticatorMethods = await graphClient.Me.Authentication.PasswordlessMicrosoftAuthenticatorMethods
    .Request()
    .GetAsync();

```