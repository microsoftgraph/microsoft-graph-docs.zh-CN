---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd8415bf9e8be5c0deca4f1d1775e70a2fedc9dc
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2Methods = await graphClient.Me.Authentication.Fido2Methods
    .Request()
    .GetAsync();

```