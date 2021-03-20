---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb81621e8310f8cfd052565ec9bc7ae3b587a7b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources["{ediscovery.userSource-id}"]
    .Request()
    .GetAsync();

```