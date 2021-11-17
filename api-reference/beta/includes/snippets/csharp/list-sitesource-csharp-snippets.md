---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5da496c236fd5d6cefd9628f804c46f29aa428d80255f882d1b91e52f7f9dcc0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"].SiteSources
    .Request()
    .GetAsync();

```