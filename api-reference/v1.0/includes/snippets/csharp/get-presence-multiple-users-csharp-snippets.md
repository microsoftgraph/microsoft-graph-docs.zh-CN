---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2da9cd4b849c35bc997a61428b834d5cda690614c082416fa61e2bc41906fb37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b"
};

await graphClient.Communications
    .GetPresencesByUserId(ids)
    .Request()
    .PostAsync();

```