---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9aabbafd21666dd099c07c7d5ba177ab02aee23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2AuthenticationMethod = await graphClient.Me.Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```