---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb1949e9a8fe640d0a9ca51f816eecae5066c3a9aebe544b49054a7e97b5fd20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = new ItemAddress
{
    AllowedAudiences = AllowedAudiences.Me,
    DisplayName = "Secret Hideout"
};

await graphClient.Users["{user-id}"].Profile.Addresses["{itemAddress-id}"]
    .Request()
    .UpdateAsync(itemAddress);

```