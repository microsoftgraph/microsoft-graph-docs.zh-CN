---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4532d658888965ce9ca7c4cebe208bde64a61d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photos = await graphClient.Groups["{group-id}"].Photos
    .Request()
    .GetAsync();

```