---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2301056fecc00c93a4625d0656db152e707f1dda
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var positions = await graphClient.Me.Profile.Positions
    .Request()
    .GetAsync();

```