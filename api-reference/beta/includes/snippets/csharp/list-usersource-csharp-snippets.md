---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c81cba24aed2870d0ce565d00d8dfa0f2ba6625fbf4d8fba97820350fffc9c73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"].UserSources
    .Request()
    .GetAsync();

```