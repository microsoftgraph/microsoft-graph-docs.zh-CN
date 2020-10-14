---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a922c31317a0d50b483b37e29359c9e1a8ce69
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.EmailMethods["3ddfcfc8-9383-446f-83cc-3ab9be4be18f"]
    .Request()
    .DeleteAsync();

```