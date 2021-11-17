---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff886cfd0871c665997ea701b2ada955fe99395758cfac75dc8749fc892390fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources["{ediscovery.userSource-id}"]
    .Request()
    .GetAsync();

```