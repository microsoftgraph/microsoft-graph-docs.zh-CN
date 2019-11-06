---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18cd3b5ef6c1b29fb2b538c868f7850ffe3dc09e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = await graphClient.Me.Profile.Phones["{id}"]
    .Request()
    .GetAsync();

```