---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8b5ac562b229080a69052f0388375496f98a310
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var asHierarchy = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .AsHierarchy()
    .Request()
    .GetAsync();

```