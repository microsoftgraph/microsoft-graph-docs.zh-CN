---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25e0fdda7c74afdd114bd0b42fec1bffb61f6208
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["fido2"]
    .Request()
    .GetAsync();

```