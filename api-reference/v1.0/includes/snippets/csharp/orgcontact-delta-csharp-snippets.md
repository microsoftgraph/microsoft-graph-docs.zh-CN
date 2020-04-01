---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5592480a8eb9ac16897ff1a6e153b026e892154
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["delta"]
    .Request()
    .GetAsync();

```