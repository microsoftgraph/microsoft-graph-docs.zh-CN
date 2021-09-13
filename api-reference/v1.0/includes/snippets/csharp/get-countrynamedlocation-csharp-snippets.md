---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e90ed6a755f5cb96b8dc3b2622f939efe34852ac6de1af8aea232c18b7e51fc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .GetAsync();

```