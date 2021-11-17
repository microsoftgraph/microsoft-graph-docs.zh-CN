---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df3711a07d41fa58e96bee7d1173f85daf6e629b01621d4b8dea457ca40b0216
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHolds = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds
    .Request()
    .GetAsync();

```