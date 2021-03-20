---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 152f7a97062d537b3f0675b2154e67f5878f9787
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Users["{user-id}"].UsageRights
    .Request()
    .Filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .GetAsync();

```