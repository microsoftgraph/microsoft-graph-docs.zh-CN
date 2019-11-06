---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2570ef7c7cc9150f9e07b9e55cfc14c7e049ffd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Projects["{id}"]
    .Request()
    .DeleteAsync();

```