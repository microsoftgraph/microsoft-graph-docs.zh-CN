---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04f70abea48af69562cebbfb6b00390dceb2a3cc
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationContextClassReference = await graphClient.Identity.ConditionalAccess.AuthenticationContextClassReferences["{authenticationContextClassReference-id}"]
    .Request()
    .GetAsync();

```