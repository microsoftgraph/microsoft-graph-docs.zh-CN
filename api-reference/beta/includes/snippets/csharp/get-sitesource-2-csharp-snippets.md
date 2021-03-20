---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 671f393f4c83528a6d442b8ec79d6f7edbd87a31
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].SiteSources["{ediscovery.siteSource-id}"]
    .Request()
    .GetAsync();

```