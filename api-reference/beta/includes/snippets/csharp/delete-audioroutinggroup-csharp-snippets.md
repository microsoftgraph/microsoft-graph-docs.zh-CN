---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b3815f403ce991960c39d9e920005863f28835f2d58e2caa28d71829df8d9a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups["{audioRoutingGroup-id}"]
    .Request()
    .DeleteAsync();

```