---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b8a0ab8a9180df662e31b6a67d70be7b9b71a46
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61031757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.SoftwareOathMethods["{softwareOathAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```