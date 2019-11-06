---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abb186a272215af36e3ba558fa7db79fcaaed555
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var anniversaries = await graphClient.Me.Profile.Anniversaries
    .Request()
    .GetAsync();

```