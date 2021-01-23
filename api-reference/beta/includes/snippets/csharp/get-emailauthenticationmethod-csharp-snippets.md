---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f6e2bcca48c68b8841dea2b99e448134aeb916
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = await graphClient.Me.Authentication.EmailMethods["3ddfcfc8-9383-446f-83cc-3ab9be4be18f"]
    .Request()
    .GetAsync();

```