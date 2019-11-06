---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7186d6ddfb192aa7897a81870e17247f5dd84709
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var labels = await graphClient.Me.InformationProtection.Policy.Labels
    .Request()
    .GetAsync();

```