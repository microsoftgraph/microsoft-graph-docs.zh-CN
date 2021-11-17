---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4d4e440f795d5da884ad34961a115a969687e357311ec8bc4159e39b76e6e06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].SiteSources
    .Request()
    .GetAsync();

```