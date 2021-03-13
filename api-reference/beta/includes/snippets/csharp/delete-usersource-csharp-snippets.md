---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 046787967a5f1c5fc30da90d38ef2a3966ba7b38
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources["{ediscovery.userSource-id}"]
    .Request()
    .DeleteAsync();

```