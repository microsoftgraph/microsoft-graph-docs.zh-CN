---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c43062156c959b4894b9c3441e1fd37b3a9d4f179a356ffa141fef1287ff2c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163150"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].SiteSources["{ediscovery.siteSource-id}"]
    .Request()
    .GetAsync();

```