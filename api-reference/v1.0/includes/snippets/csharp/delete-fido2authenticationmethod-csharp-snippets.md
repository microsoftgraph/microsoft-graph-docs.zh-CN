---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb591f3a808b258cfaa3466423175c9f6c852053
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```