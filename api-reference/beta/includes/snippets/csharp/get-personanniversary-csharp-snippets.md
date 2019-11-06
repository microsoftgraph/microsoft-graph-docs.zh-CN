---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff9e28a2c3abbbd6596f489b2d05db252f47218
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnniversary = await graphClient.Me.Profile.Anniversaries["{id}"]
    .Request()
    .GetAsync();

```