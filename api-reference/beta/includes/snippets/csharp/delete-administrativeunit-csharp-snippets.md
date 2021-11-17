---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23db6215cee7553b622751c1dea83a7196fea2e3b08799b88a54bc599d5507f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .DeleteAsync();

```