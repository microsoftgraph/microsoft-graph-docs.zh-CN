---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb52ef62b81320f0e1053573f43697199d617560
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475323"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["microsoftAuthenticator"]
    .Request()
    .GetAsync();

```