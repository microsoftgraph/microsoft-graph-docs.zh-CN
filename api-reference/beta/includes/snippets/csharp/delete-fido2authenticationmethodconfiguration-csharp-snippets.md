---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f478fc66d7285956183e22b7d42069cf27742a0e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["fido2"]
    .Request()
    .DeleteAsync();

```