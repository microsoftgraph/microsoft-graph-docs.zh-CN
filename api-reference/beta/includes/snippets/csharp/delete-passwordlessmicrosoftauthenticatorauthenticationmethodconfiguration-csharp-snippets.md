---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7facc676d9fd528e32d413acd532af77c28def47
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["passwordlessMicrosoftAuthenticator"]
    .Request()
    .DeleteAsync();

```