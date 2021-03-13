---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb591f3a808b258cfaa3466423175c9f6c852053
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```