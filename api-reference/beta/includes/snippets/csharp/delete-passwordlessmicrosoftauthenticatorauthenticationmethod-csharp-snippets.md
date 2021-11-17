---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 370a5cf7db2168b5d4140e89e0f208adda09d9421715dbf0f70e632b9b6fea0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.PasswordlessMicrosoftAuthenticatorMethods["{passwordlessMicrosoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```