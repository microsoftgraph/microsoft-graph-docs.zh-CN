---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a25bf9dba4a27715a2b30674b21207b1014ffc1dab2d3ee29ee67fb030e90716
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = await graphClient.AdministrativeUnits
    .Request()
    .GetAsync();

```