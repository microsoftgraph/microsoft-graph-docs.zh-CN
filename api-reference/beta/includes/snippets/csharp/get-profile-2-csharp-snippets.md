---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae9f17057a1717136eb03eda4fb5974f837a95b565e775065562b5415db1ad5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profile = await graphClient.Me.Profile
    .Request()
    .Expand("skills($select=displayName)")
    .GetAsync();

```