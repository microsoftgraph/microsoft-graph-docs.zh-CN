---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 604bcd85fd849b8f674bfb2f8c543b2ecf4d87c09b8999d60a939d335f6a5fb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218754"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.MicrosoftAuthenticatorMethods["{microsoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```