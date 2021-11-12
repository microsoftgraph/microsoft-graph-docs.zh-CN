---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8315a379a8eea9050c8dc3c93a460ebe9781c2cdb465170be197558fe064048
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = new ItemPhone
{
    Type = PhoneType.Other
};

await graphClient.Users["{user-id}"].Profile.Phones["{itemPhone-id}"]
    .Request()
    .UpdateAsync(itemPhone);

```