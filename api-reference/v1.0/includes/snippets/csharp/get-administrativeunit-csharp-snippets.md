---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04d86be8cd6b460b418a145d3789fb3708a2031
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .GetAsync();

```