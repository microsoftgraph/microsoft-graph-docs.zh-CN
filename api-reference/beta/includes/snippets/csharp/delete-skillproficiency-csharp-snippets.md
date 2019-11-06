---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d37d4433aeefd1220200fd92f0b9005888268b1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Skills["{id}"]
    .Request()
    .DeleteAsync();

```