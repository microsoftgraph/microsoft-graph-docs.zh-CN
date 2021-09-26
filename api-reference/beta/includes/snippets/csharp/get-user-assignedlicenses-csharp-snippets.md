---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78618c04166e71583d5c4222d0dd8d39e58badce
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)")
    .Select("id,mail,assignedLicenses")
    .GetAsync();

```