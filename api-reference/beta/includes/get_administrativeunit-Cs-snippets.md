---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a69d2da81478dc62e3a698ab4890a9d0b283050
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Education.Schools["2961761D-8094-4183-A9F6-8E36E966C7D9"].AdministrativeUnit
    .Request()
    .GetAsync();

```