---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdeed8a0a7a8fb294ca9cc51140e420fde6cf6b7024889c38429ff7d81e866b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    Nickname = "Kesha"
};

await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .UpdateAsync(personName);

```