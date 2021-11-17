---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f8ef920610fd554ef51ecf3806ce7155e70708a53ff2c9f2b6af4f0fc94918
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162501"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Activate()
    .Request()
    .PostAsync();

```